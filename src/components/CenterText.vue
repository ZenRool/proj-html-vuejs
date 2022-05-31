<template>
  <div
    class="center-text container container-small d-flex align-items-center flex-column"
  >
    <img
      v-if="elem.icon !== 0"
      :src="require(`../assets/images/icon-${elem.icon}.png`)"
      alt="icon"
    />
    <h2 :class="{ caps: elem.icon !== 0 }">{{ elem.title }}</h2>
    <div v-if="elem.line" class="line"></div>
    <p>{{ elem.paragraph }}</p>
  </div>
</template>
<script>
export default {
  name: "CenterText",
  props: {
    elem: {
      icon: Number,
      title: String,
      paragraph: String,
      line: Boolean,
    },
  },
};
</script>
<style lang="scss" scoped>
@import "../style/variables.scss";
* {
  margin: 1.2rem 0;
  text-align: center;
}
.center-text {
  padding-top: 3rem;
  p {
    line-height: 2.5rem;
    font-size: 1.1rem;
  }
  .line {
    height: 0;
    width: 50%;
    border-bottom: 1px solid $reven;
  }
  img {
    width: 80px;
    height: 80px;
  }
  .caps {
    text-transform: uppercase;
  }
}
</style>
