<template>
  <div class="home-container">
    <h1>{{ msg }}</h1>
    <img src="../../assets/images/what-the-duck.jpg" alt="">
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Home extends Vue {
  @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.home-container {
  text-align: center;
}
h1 {
  color: #2c3e50;
  margin-top: 60px;
}

img {
  height: 400px;
  width: 400px;
}
</style>
