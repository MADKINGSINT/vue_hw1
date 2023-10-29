<template>
  <div>
    <div class="top">
      <img src="../assets/img/Photo.jpg" alt="" />
    </div>
    <div class="about">
      <h1 class="about__title">{{ title }}</h1>
      <p class="about__text">{{ text1 }}</p>
      <p class="about__text">{{ text2 }}</p>
    </div>
    <h1>{{ string1 }}</h1>
    <Slider ></Slider>
  </div>

</template>

<script>
import { mapState } from "vuex";
import Slider from './Carusel.vue';
export default {
  computed: {
    ...mapState(["title", "text1", "text2"]),
    },
    components: {
        Slider,
    },
  data() {
    return {
        currentSlide: 0,

    };
    },
  

};
</script>

<style lang="scss" scoped>
.about {
  padding-top: 100px;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  flex-direction: column;
  align-content: center;
  align-items: center;
  &__title {
    color: #292f36;
    font-family: DM Serif Display;
    font-size: 50px;
    font-style: normal;
    font-weight: 400;
    line-height: 125%; /* 62.5px */
    letter-spacing: 1px;
  }
  &__text {
    width: 658px;
    color: #4d5053;
    font-family: Jost;
    font-size: 22px;
    font-style: normal;
    font-weight: 400;
    line-height: 150%; /* 33px */
    letter-spacing: 0.22px;
  }

}
</style>
