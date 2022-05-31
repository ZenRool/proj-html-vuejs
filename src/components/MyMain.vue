<template>
  <main id="about">
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
    <section class="background-gray">
      <CenterText :elem="this.bigElement[1]" />
      <div
        class="container container-regular d-flex justify-content-between my-1"
      >
        <DocCard v-for="elem in this.doctors" :key="elem.doctor" :elem="elem" />
      </div>
    </section>
    <section>
      <CenterText :elem="this.bigElement[2]" />
      <div class="container container-regular d-flex wrap">
        <MiniCenterText
          v-for="elem in this.service"
          :key="elem.icon"
          :elem="elem"
          class="third"
        />
      </div>
    </section>
  </main>
</template>
<script>
import CenterText from "./CenterText.vue";
import MiniCenterText from "./MiniCenterText.vue";
import DocCard from "./DocCard.vue";
export default {
  name: "MyMain",
  components: {
    CenterText,
    MiniCenterText,
    DocCard,
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
        {
          icon: 5,
          title: "Meet our doctors",
          line: true,
          paragraph:
            "Sed ut perspiciatis unde omnis iste naus error sit voluptatem accusatium doloremque ladantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae",
        },
        {
          icon: 6,
          title: "our healthservices",
          line: true,
          paragraph:
            "Sed ut perspiciatis unde omnis iste naus error sit voluptatem accusatium doloremque ladantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae",
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
      service: [
        {
          icon: 14,
          title: "rehabilitation cener",
          paragraph:
            "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis prasentium voluptatum deleniti atque corrupti quos dolores et quas",
        },
        {
          icon: 15,
          title: "World class facilities",
          paragraph:
            "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis prasentium voluptatum deleniti atque corrupti quos dolores et quas",
        },
        {
          icon: 16,
          title: "Expert doctors",
          paragraph:
            "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis prasentium voluptatum deleniti atque corrupti quos dolores et quas",
        },
        {
          icon: 11,
          title: "Complementary therapies",
          paragraph:
            "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis prasentium voluptatum deleniti atque corrupti quos dolores et quas",
        },
        {
          icon: 12,
          title: "Complementary therapies",
          paragraph:
            "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis prasentium voluptatum deleniti atque corrupti quos dolores et quas",
        },
        {
          icon: 13,
          title: "Complementary therapies",
          paragraph:
            "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis prasentium voluptatum deleniti atque corrupti quos dolores et quas",
        },
      ],
      doctors: [
        {
          doctor: 1,
          docName: "jon snow",
          title: "Anesthesiologist",
          paragraph:
            "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis prasentium voluptatum deleniti atque",
        },
        {
          doctor: 2,
          docName: "tony stark",
          title: "Cardiologist",
          paragraph:
            "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis prasentium voluptatum deleniti atque",
        },
        {
          doctor: 3,
          docName: "anna smith",
          title: "Nurse Practitioner",
          paragraph:
            "At vero eos et accusamus et iusto odio dignissimos ducimus qui blanditiis prasentium voluptatum deleniti atque",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
main {
  section {
    padding: 2rem 0;
    .third {
      width: calc(100% / 3);
    }
  }
}
</style>
