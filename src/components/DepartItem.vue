<template>
  <li class="d-flex">
    <div>
      <i class="fa-solid fa-chevron-right"></i>
    </div>
    {{ elem }}
  </li>
</template>
<script>
export default {
  name: "ContactItem",
  props: {
    elem: String,
  },
};
</script>
<style lang="scss" scoped>
@import "../style/variables.scss";
li {
  margin: 1.2rem 0;
  text-align: center;
  line-height: 1.8rem;
  font-size: 0.9rem;
  div {
    color: white;
    background-color: $pelorous;
    width: 1.8rem;
    height: 1.8rem;
    text-align: center;
    margin-right: 1rem;
    border-radius: 50%;
  }
}
</style>
