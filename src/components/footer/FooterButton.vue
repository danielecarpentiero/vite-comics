<template>
  <button>{{ buttonText }}</button>
</template>

<script>
export default {
  name: "FooterButton",
  data() {
    return {
      buttonText: "sign up now!",
    };
  },
};
</script>

<style scoped lang="scss">
@use "src/styles/variables.scss" as *;
button {
  width: 10%;
  height: 4vh;
  background-color: $lighter--secondary--color;
  border: 2px solid $complementary--color;
  text-transform: uppercase;
  color: $primary--color;
  font-size: 1rem;
  font-weight: 700;
}
</style>
