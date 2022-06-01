<template>
  <div
    class="cardiogram container container-small d-flex align-items-center flex-column"
    :class="elem.color"
  >
    <h4>{{ elem.title }}</h4>
    <img src="../assets/images/wave-divider.png" alt="cardiogram" />
    <p>{{ elem.paragraph }}</p>
    <div class="learn">Learn more</div>
  </div>
</template>
<script>
export default {
  name: "CardiogramText",
  props: {
    elem: {
      title: String,
      paragraph: String,
      color: String,
    },
  },
};
</script>
<style lang="scss" scoped>
@import "../style/variables.scss";
* {
  text-align: center;
  margin: 0.8rem 0;
}
.pelorous {
  background-color: $pelorous;
  &-variant {
    background-color: $pelorous-variant;
  }
  &-dark {
    background-color: $pelorous-dark;
  }
}
.cardiogram {
  padding: 1.5rem 0;
  color: white;
  p {
    line-height: 2.5rem;
    font-size: 0.9rem;
  }
  .line {
    height: 0;
    width: 50%;
    border-bottom: 1px solid $reven;
    border-bottom-color: currentColor;
  }
  img {
    width: 100px;
    height: 30px;
  }
  .learn {
    text-transform: uppercase;
    border: 2px solid white;
    padding: 0.8rem 2.5rem;
    font-size: 1.1rem;
    cursor: pointer;
    &:hover {
      background-color: $pelorous-vibrant;
      border-color: gallery;
      color: gallery;
    }
  }
}
</style>
