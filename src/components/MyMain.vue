<template>
  <main id="departments">
    <section>
      <CenterText :elem="this.bigElement[0]" />
      <div class="container container-regular d-flex">
        <MiniCenterText
          v-for="elem in this.welcome"
          :key="elem.icon"
          :elem="elem"
        />
      </div>
    </section>
  </main>
</template>
<script>
import CenterText from "./CenterText.vue";
import MiniCenterText from "./MiniCenterText.vue";
export default {
  name: "MyMain",
  components: {
    CenterText,
    MiniCenterText,
  },
  data: function () {
    return {
      bigElement: [
        {
          icon: 0,
          title: "Welcome to Avada Health",
          line: false,
          paragraph:
            "Sed ut perspiciatis unde omnis iste naus error sit voluptatem accusatium doloremque ladantium, totam rem aperiam, eaque ipsa quae ab illo",
        },
      ],
      welcome: [
        {
          icon: 1,
          title: "Same day appointments",
          paragraph:
            "Sed ut perspiciatis unde omnis iste naus error sit voluptatem accusatium",
        },
        {
          icon: 2,
          title: "World class facilities",
          paragraph:
            "Sed ut perspiciatis unde omnis iste naus error sit voluptatem accusatium",
        },
        {
          icon: 3,
          title: "Expert doctors",
          paragraph:
            "Sed ut perspiciatis unde omnis iste naus error sit voluptatem accusatium",
        },
        {
          icon: 4,
          title: "Complementary therapies",
          paragraph:
            "Sed ut perspiciatis unde omnis iste naus error sit voluptatem accusatium",
        },
      ],
    };
  },
};
</script>
