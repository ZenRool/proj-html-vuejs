<template>
  <div id="app">
    <HeaderJumbo />
  </div>
</template>

<script>
import HeaderJumbo from "./components/HeaderJumbo.vue";
export default {
  name: "App",
  components: {
    HeaderJumbo,
  },
};
</script>

<style lang="scss">
@import "./style/common.scss";
@import "./style/variables.scss";
</style>
