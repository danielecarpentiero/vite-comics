<template>
  <div>
    <img :src="slide" alt="" />
    <h3>{{ title }}</h3>
  </div>
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
img {
  width: 200px;
  height: 200px;
  object-fit: cover;
  object-position: top;
  display: block;
}
</style>
