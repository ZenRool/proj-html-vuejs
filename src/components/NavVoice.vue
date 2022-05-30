<template>
  <li>
    <a :href="`#${voice.split(' ')[0]}`">{{ voice }}</a>
  </li>
</template>
<script>
export default {
  name: "NavVoice",
  props: {
    voice: String,
  },
};
</script>
<style lang="scss" scoped>
@import "../style/variables.scss";
a:hover {
  color: $pelorous;
}
</style>
