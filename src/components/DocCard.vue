<template>
  <div class="card">
    <div class="pic">
      <img
        :src="require(`../assets/images/doctor-${elem.doctor}.jpg`)"
        :alt="elem.docName"
      />
    </div>
    <div class="info">
      <h3>{{ elem.docName }}</h3>
      <p class="title">{{ elem.title }}</p>
      <p class="paragraph">{{ elem.paragraph }}</p>
    </div>
  </div>
</template>
<script>
export default {
  name: "CenterText",
  props: {
    elem: {
      doctor: Number,
      docName: String,
      title: String,
      paragraph: String,
    },
  },
};
</script>
<style lang="scss" scoped>
.card {
  background: white;
  height: 740px;
  width: 359px;
  .pic {
    height: 50%;
    img {
      display: block;
      object-fit: contain;
      height: 100%;
      width: 100%;
    }
  }
  .info {
    padding: 1.6rem;
    h3 {
      margin: 0.8rem 0;
    }
    .title {
      margin-bottom: 2.4rem;
    }
    .paragraph {
      line-height: 2rem;
    }
  }
}
</style>
