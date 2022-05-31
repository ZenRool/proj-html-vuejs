<template>
  <section id="home">
    <MyHeader />
    <div
      class="container container-regular d-flex flex-column justify-content-center"
    >
      <h1>Caring <span class="text-blue">For Life</span></h1>
      <p class="my-1">
        Kind words can be short and easy to speak, but their echoes are truly
        endless. Avada Health focuses on you as if it was our own family.
      </p>
      <p>
        <a href="#" class="button-blue">Learn more</a>
      </p>
    </div>
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
div {
  height: 100%;
  p {
    font-size: 1.4rem;
    width: 70%;
  }
  .button-blue {
    padding-top: 0.5rem;
    padding-bottom: 0.5rem;
  }
}
</style>
