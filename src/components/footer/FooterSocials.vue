<template>
  <div class="footer-socials">
    <h3>follow us</h3>
    <ul>
      <li v-for="item in socials">
        <a :href="item.link" :target="item.target">
          <img :src="item.icon" :alt="item.icon" />
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "FooterSocials",
  data() {
    return {
      socials: [
        {
          icon: "src/assets/img/footer-facebook.png",
          link: "#",
          target: "_blank",
        },
        {
          icon: "src/assets/img/footer-twitter.png",
          link: "#",
          target: "_blank",
        },
        {
          icon: "src/assets/img/footer-youtube.png",
          link: "#",
          target: "_blank",
        },
        {
          icon: "src/assets/img/footer-pinterest.png",
          link: "#",
          target: "_blank",
        },
        {
          icon: "src/assets/img/footer-periscope.png",
          link: "#",
          target: "_blank",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@use "src/styles/variables.scss" as *;
.footer-socials {
  display: flex;
  flex-direction: row;
  align-items: center;
}
ul {
  display: flex;
}
h3 {
  text-transform: uppercase;
  color: $complementary--color;
  font-size: 20px;
  margin-bottom: 20px;
}

li {
  list-style: none;
  padding: 10px;
}
</style>
