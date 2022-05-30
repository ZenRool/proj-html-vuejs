<template>
  <div id="app">
    <HeaderJumbo />
    <MyMain />
  </div>
</template>

<script>
import HeaderJumbo from "./components/HeaderJumbo.vue";
import MyMain from "./components/MyMain.vue";
export default {
  name: "App",
  components: {
    HeaderJumbo,
    MyMain,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
@import "./style/variables.scss";
</style>
