<template>
  <main id="departments">
    <CenterText :elem="this.bigElement[0]" />
  </main>
</template>
<script>
import CenterText from "./CenterText.vue";
export default {
  name: "MyMain",
  components: {
    CenterText,
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
    };
  },
};
</script>
