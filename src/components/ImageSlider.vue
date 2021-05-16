<template>
  <vueper-slides
    :dragging-distance="70"
    prevent-y-scroll
    :breakpoints="breakpoints"
    :pause-on-hover="pauseOnHover"
  >
    <vueper-slide
      v-for="(slide, i) in slides"
      :key="i"
      :image="slide.image"
      :title="slide.title"
      :content="slide.content"
    />
  </vueper-slides>
</template>
<script>
import { VueperSlides, VueperSlide } from "vueperslides"
import "vueperslides/dist/vueperslides.css"

export default {
  name: "ImageSlider",
  components: { VueperSlides, VueperSlide },
  data: () => ({
    breakpoints: {
        425: {
            slideRatio: 1 / 1,
            arrows: false,
            bulletsOutside: true
        },
        768: {
            slideRatio: 1 / 2,
            arrows: false,
            bulletsOutside: true
        }
    },
    slides: [
        {
            title: "<h2>Slide 1 title</h2>",
            content: 'Slide content <b>with bold styling</b>.',
            image: require('@/assets/asset-1.jpg')
        },
        {
            title: '<h2>Slide 2 title</h2>',
            content: 'Slide content <i>with italic styling</i>..',
            image: require('@/assets/asset-2.jpg')
        },
        {
            title: '<h2>Slide 3 title</h2>',
            content: 'Slide content with no styling.',
            image: require('@/assets/asset-3.jpg')
        },
        {
            title: '<h2>Slide 4 title</h2>',
            content: `<p>Slide content</p><p>With multiple paragraphs.</p>`,
            image: require('@/assets/asset-4.jpg')
        },
    ],
    pauseOnHover: true
  })
};
</script>


<style lang="stylus">
.vueperslides {
  & .vueperslide__title {
    color: white;
    font-size: 40px;
    text-shadow: 0px 0px 3px black;
  }

  & .vueperslide__content {
    color: white;
    font-size: 25px;
    text-shadow: 0px 0px 3px black;

    & p {
      padding-bottom: 10px;
    }
  }

  & .vueperslides__arrow {
    & svg {
      border-radius: 50%;
      color: white;
      border: 1px solid white;
      height: 60px;
      width: 60px;
      stroke-width: 2;
      opacity: 1;

      &:hover {
        color: rgba(0, 128, 0, 100%);
        background-color: rgba(255, 255, 255, 50%);
        border: 1px solid green;
      }
    }
  }
}
</style>