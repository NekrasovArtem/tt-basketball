<script setup>
import { onMounted, ref, watch } from "vue";

const sliderBackground = ref(null);
const sliderIndex = ref(1);
// eslint-disable-next-line
const slides = ["играй", "учись", "смотри"];

onMounted(() => {
  setSliderBackground();
});

watch(sliderIndex, setSliderBackground);

function setSliderBackground() {
  if (window.innerWidth < 768) {
    sliderBackground.value.src = `./img/slider_photo_mobile_${sliderIndex.value}.webp`;
  } else {
    sliderBackground.value.src = `./img/slider_photo_${sliderIndex.value}.webp`;
  }
}
</script>

<template lang="pug">
section.section.section__slider
  img.slider__background(ref="sliderBackground")
  .slider__wrapper 
    h2.section__title.slider__title="Найди с кем поиграть в баскет"
    .slider__menu 
      .slider__item(v-for="(item, index) in slides" @mouseenter="sliderIndex = index + 1")
        span.item__text {{ item }}
        img.slider__arrow(src="../assets/img/white_arrow.svg", alt="Подробнее")
</template>

<style lang="scss"></style>
