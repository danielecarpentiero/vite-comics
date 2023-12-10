<template>
  <div class="container">
    <ul>
      <li v-for="object in objects">
        <img :src="object.picture" alt="" />{{ object.title }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "AdsMain",
  data() {
    return {
      objects: [
        {
          picture: "src/assets/img/buy-comics-digital-comics.png",
          title: "digital comics",
        },
        {
          picture: "src/assets/img/buy-comics-merchandise.png",
          title: "dc merchandise",
        },
        {
          picture: "src/assets/img/buy-comics-subscriptions.png",
          title: "subscriptions",
        },
        {
          picture: "src/assets/img/buy-comics-shop-locator.png",
          title: "comic shop locator",
        },
        {
          picture: "src/assets/img/buy-dc-power-visa.svg",
          title: "dc power visa",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@use "src/styles/variables.scss" as *;
.container {
  width: 75%;
  ul {
    list-style: none;
    display: flex;
    li {
      width: 100%;
      display: flex;
      align-items: center;
      text-transform: uppercase;
      color: $primary--color;
      font-size: 20px;
      cursor: pointer;
      img {
        height: 30%;
        margin-right: 20px;
      }
    }
  }
}
</style>
