<template>
  <div id="app">
    <HeaderJumbo />
    <MyMain />
    <MyFooter />
  </div>
</template>
<script>
import HeaderJumbo from "./components/HeaderJumbo.vue";
import MyMain from "./components/MyMain.vue";
import MyFooter from "./components/MyFooter.vue";
export default {
  name: "App",
  components: {
    HeaderJumbo,
    MyMain,
    MyFooter,
  },
};
</script>
<style lang="scss">
@import "./style/common.scss";
@import "./style/variables.scss";
</style>
