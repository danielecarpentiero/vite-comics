<template>
  <div class="jumbotron">
    <img :src="image" :alt="title" />
  </div>
  <SliderVue />
</template>

<script>
import SliderVue from "./Slider.vue";
export default {
  name: "JumboMain",
  data() {
    return {
      image: "src/assets/img/jumbotron.jpg",
      title: "teen-titans",
    };
  },
  components: {
    SliderVue,
  },
};
</script>

<style scoped lang="scss">
@use "src/styles/variables.scss" as *;
.jumbotron {
  img {
    width: 100%;
    height: 400px;
    object-fit: cover;
    object-position: top;
  }
}
</style>
