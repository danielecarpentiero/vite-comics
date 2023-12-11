<template>
  <figure>
    <img :src="slide" alt="slide" />
  </figure>
  <h3>{{ title }}</h3>
</template>

<script>
export default {
  name: "Slide",
  props: {
    slide: String,
    title: String,
    genre: String,
  },
};
</script>

<style scoped lang="scss">
@use "src/styles/variables.scss" as *;

figure {
  height: 200px;
  cursor: pointer;
}

img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: top;
  display: block;
}
</style>
