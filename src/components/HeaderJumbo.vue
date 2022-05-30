<template>
  <section id="home">
    <MyHeader />
  </section>
</template>
<script>
import MyHeader from "./MyHeader.vue";
export default {
  name: "HeaderJumbo",
  components: {
    MyHeader,
  },
};
</script>
<style lang="scss" scoped>
section {
  height: 860px; // ?
  background-image: url("../assets/images/header-image-homepage.jpg");
  color: white;
}
</style>
