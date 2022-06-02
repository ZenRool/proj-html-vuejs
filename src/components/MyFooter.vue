<template>
  <footer>
    <div class="footer-top d-flex container container-large">
      <section class="third">
        <img
          src="../assets/images/medical_logo_1x_dark.png"
          alt="Medical Logo"
        />
        <p>
          Sed ut perspiciatis unde omnis iste naus error sit voluptatem
          accusatium dolemue ladantium totam aperiam, eaque ipsa quae ab illo
          inventore veritatis et quasi architecto beatae luptatem
          accusantium,remaperiamsiat. Voluptatem accusest etsium doloremque
          laudaien. Lorem ipsum sits dolores ets unser.
        </p>
        <div class="line"></div>
        <div class="learn">learn more about us</div>
        <div class="my-1 d-flex">
          <SocialSquere
            v-for="(social, index) in this.socials"
            :key="index"
            :social="social"
            class="mr-1"
          />
        </div>
      </section>
    </div>
  </footer>
</template>
<script>
import SocialSquere from "./SocialSquere.vue";
export default {
  name: "App",
  components: {
    SocialSquere,
  },
  data: function () {
    return {
      socials: ["facebook", "twitter", "instagram", "youtube"],
    };
  },
};
</script>
<style lang="scss">
@import "../style/variables.scss";
.footer-top {
  padding: 4rem 0;
  img {
    max-height: 100px;
    width: auto;
  }
  p {
    line-height: 3rem;
    font-size: 0.9rem;
    margin: 0.7rem 0;
  }
  .line {
    width: 100%;
    border-bottom: 1px solid $river-bed;
  }
  .learn {
    text-transform: uppercase;
    font-size: 1.1rem;
    margin: 0.5rem 0;
  }
}
</style>
