<template>
  <li>
    <span><i :class="`fas fa-${elem.type}`"></i></span> {{ elem.value }}
  </li>
</template>
<script>
export default {
  name: "ContactItem",
  props: {
    elem: {
      type: String,
      value: String,
    },
  },
};
</script>
<style lang="scss" scoped>
@import "../style/variables.scss";
li {
  margin: 1rem 0;
  span {
    color: $pelorous;
    font-size: 1.1rem;
    display: inline-block;
    width: 2rem;
  }
}
</style>
