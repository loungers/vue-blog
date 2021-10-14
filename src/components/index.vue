<template>
  <div class="main">
    <div class="top">
      <div class="logo"></div>
      <div class="left"></div>
      <div class="center"></div>
      <div class="right"></div>
      <div class="buttom"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Index",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.main {
  height: 100vh;
  // width: auto;
  background: url("../assets/images/background.jpg") no-repeat center center
    fixed;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;

  .top {
    padding: 1.5em;
    
    .logo {
      margin: 0 auto;
      width: 98%;
      height: 4em;
      border-radius: 15px;
      // background: #d0d6ee; /*注释后变透明*/
      box-shadow: 18px 18px 35px #f0eff7, -18px -18px 35px #ffffff;
    }
  }
}
</style>
