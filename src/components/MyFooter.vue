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
      <section class="third">
        <h3>Contact Information</h3>
        <div class="line-small"></div>
        <ul>
          <ContactItem
            v-for="(item, index) in this.contacts"
            :key="index"
            :elem="item"
          />
        </ul>
      </section>
    </div>
  </footer>
</template>
<script>
import SocialSquere from "./SocialSquere.vue";
import ContactItem from "./ContactItem.vue";
export default {
  name: "App",
  components: {
    SocialSquere,
    ContactItem,
  },
  data: function () {
    return {
      socials: ["facebook", "twitter", "instagram", "youtube"],
      contacts: [
        {
          type: "map-marker-alt",
          value: "121 King Street, London United Kingdom",
        },
        {
          type: "phone-flip",
          value: "1.800.458.556",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
@import "../style/variables.scss";
.footer-top {
  padding: 4rem 0;
  .third {
    padding: 1rem;
  }
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
    &-small {
      width: 10%;
      border-bottom: 2px solid $pelorous;
      margin: 2rem 0;
    }
  }
  .learn {
    text-transform: uppercase;
    font-size: 1.1rem;
    margin: 0.5rem 0;
  }
}
</style>
