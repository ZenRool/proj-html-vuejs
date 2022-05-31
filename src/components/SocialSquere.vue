<template>
  <div :class="this.social" class="squere">
    <i
      class="fab"
      :class="`fa-${this.social}${this.social === 'facebook' ? '-f' : ''}`"
    ></i>
  </div>
</template>
<script>
export default {
  name: "SocialSquere",
  props: {
    social: String,
  },
};
</script>
<style lang="scss" scoped>
@import "../style/variables.scss";
@import "~@fortawesome/fontawesome-free/css/all.min.css";
.squere {
  color: white;
  height: 2rem;
  width: 2rem;
  font-size: 1.1rem;
  line-height: 2rem;
  text-align: center;
  border-radius: 5px;
}
.facebook {
  background-color: $facebook;
}
.instagram {
  background-color: $facebook;
}
.twitter {
  background-color: $twitter;
}
.youtube {
  background-color: $thunderbird;
}
</style>
