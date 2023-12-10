<template>
  <footer>
    <div class="container">
      <FooterButton />
      <FooterSocials />
    </div>
  </footer>
</template>

<script>
import FooterButton from "./FooterButton.vue";
import FooterSocials from "./FooterSocials.vue";
export default {
  name: "LowerFooter",
  components: {
    FooterButton,
    FooterSocials,
  },
};
</script>

<style scoped lang="scss">
@use "src/styles/variables.scss" as *;
footer {
  padding: 20px 0;
  background-color: $lighter--secondary--color;
  width: 100%;
  display: flex;
  justify-content: center;

  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 75%;
  }
}
</style>
