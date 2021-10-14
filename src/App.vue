<template>
  <div id="app">
    <!--    <img alt="Vue logo" src="./assets/logo.png">-->
    <!--    <HelloWorld msg="Welcome to Your Vue.js App"/>-->
    <Index />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Index from "./components";

export default {
  name: "App",
  components: {
    // HelloWorld,
    Index,
  },
};
</script>

<style scope lang="scss">
* {
  margin: 0;
  padding: 0;
}
body {
  margin: 0;
  #app {
    height: 100%;
    width: 100%;
  }
}
</style>
