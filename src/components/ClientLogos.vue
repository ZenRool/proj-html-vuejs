<template>
  <div class="carro container container-regular d-flex">
    <div class="container container-regular d-flex">
      <div class="image" v-for="icon in this.icons" :key="icon">
        <img
          :src="require(`../assets/images/client-logos-${icon}.png`)"
          alt="client"
        />
      </div>
    </div>
    <div class="container container-regular d-flex">
      <div class="image" v-for="icon in this.icons" :key="icon">
        <img
          :src="require(`../assets/images/client-logos-${icon}.png`)"
          alt="client"
        />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "ClientLogos",
  data: function () {
    return {
      icons: [1, 2, 3, 4],
    };
  },
};
</script>
<style lang="scss" scoped>
.carro {
  overflow-x: hidden;
  .image {
    width: 300px;
    height: 300px;
    position: relative;
    animation: move 7s infinite linear;
  }
  @keyframes move {
    from {
      left: 0px;
    }
    to {
      left: -1130px;
    }
  }
}
</style>
