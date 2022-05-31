<template>
  <div
    class="center-text container container-small d-flex align-items-center flex-column"
  >
    <img :src="require(`../assets/images/icon-${elem.icon}.png`)" alt="icon" />
    <h3>{{ elem.title }}</h3>
    <p>{{ elem.paragraph }}</p>
  </div>
</template>
<script>
export default {
  name: "MiniCenterText",
  props: {
    elem: {
      icon: Number,
      title: String,
      paragraph: String,
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
div {
  margin-top: 2.5rem;
  padding: 0 0.5rem;
  p {
    line-height: 2rem;
    font-size: 0.9rem;
  }
  img {
    width: 80px;
    height: 80px;
  }
}
</style>
