<template>
  <div class="jumbotron">
    <img :src="image" :alt="title" />
    <div class="btn">current series</div>
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
  position: relative;
  img {
    width: 100%;
    height: 400px;
    object-fit: cover;
    object-position: top;
    display: block;
  }
  .btn {
    background-color: $complementary--color;
    text-transform: uppercase;
    padding: 10px;
    color: $primary--color;
    width: 200px;
    text-align: center;
    font-size: 1.5rem;
    position: absolute;
    bottom: -20px;
    left: 10%;
    font-weight: 700;
    cursor: pointer;
  }
}
</style>
