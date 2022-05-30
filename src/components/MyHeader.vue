<template>
  <header
    class="container container-large d-flex justify-content-between align-items-center"
  >
    <div>
      <img src="../assets/images/medical_logo_1x_light.png" alt="icon" />
    </div>
    <nav>
      <ul class="d-flex">
        <NavVoice
          v-for="(voice, index) in this.voices"
          :key="index"
          :voice="voice"
          :class="{ 'button-blue': index == voices.length - 1 }"
        />
      </ul>
    </nav>
  </header>
</template>
<script>
import NavVoice from "./NavVoice.vue";
export default {
  name: "MyHeader",
  components: {
    NavVoice,
  },
  data: function () {
    return {
      voices: ["home", "about", "departments", "articles", "make appointment"],
    };
  },
};
</script>
<style lang="scss" scoped>
header {
  height: 80px;
  img {
    height: 50px;
  }
  li {
    font-size: 0.9rem;
    margin-left: 1.5rem;
    text-transform: uppercase;
    height: 40px;
    line-height: 40px;
  }
}
</style>
