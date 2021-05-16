<template>
  <ImageSlider />
  <IntroText />
</template>

<script>
// @ is an alias to /src
import ImageSlider from "@/components/ImageSlider.vue";
import IntroText from "@/components/IntroText.vue";

export default {
  name: "Home",
  components: {
    ImageSlider,
    IntroText,
  },
};
</script>
