<template>
  <footer>
    <div class="container footer-container">
      <div class="footer-links-container">

        <div class="dc-comics-links">
          <div class="title-links">DC COMICS</div>
          <a href="#!" v-for="link in dcComicsLinks" :key="link">{{ link.text }}</a>
        </div>

        <div class="dc-comics-links">
          <div class="title-links">DC</div>
          <a href="#!" v-for="link in dcLinks" :key="link"> {{ link.text }} </a>
        </div>

        <div class="dc-comics-links">
          <div class="title-links">SITE</div>
          <a href="#!" v-for="link in siteLinks" :key="link">{{ link.text }} </a>
        </div>

        <div class="dc-comics-links shop-links">
          <div class="title-links">SHOP</div>
          <a href="#!" v-for="link in shopLinks" :key="link">{{ link.text }}</a>
        </div>

      </div>

      <img class="dc-logo-background" src="../../src/assets/img/dc-logo-bg.png" alt="">
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterDc",
  data() {
    return {
      dcComicsLinks: [
        {
          text: "Caracthers",
        },
        {
          text: "Comics",
        },
        {
          text: "Movies",
        },
        {
          text: "Tv",
        },
        {
          text: "Games",
        },
        {
          text: "Videos",
        },
        {
          text: "News",
        },
      ],
      dcLinks: [
        {
          text: "Terms of Use",
        },
        {
          text: "Privacy Policy (New)",
        },
        {
          text: "Add Choices",
        },
        {
          text: "Advertising",
        },
        {
          text: "Jobs",
        },
        {
          text: "Subscriptions",
        },
        {
          text: "Talent Workshops",
        },
        {
          text: "CPSP Certificates",
        },
        {
          text: "Ratings",
        },
        {
          text: "Shop Help",
        },
        {
          text: "Contact Us",
        },
      ],
      siteLinks: [
        {
          text: "DC",
        },
        {
          text: "MAD Magazine",
        },
        {
          text: "DC Kids",
        },
        {
          text: "DC Universe",
        },
        {
          text: "DC Power VISA",
        },
      ],
      shopLinks: [
        {
          text: "Shop DC",
        },
        {
          text: "Shop DC Collectibles",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
footer {
  width: 100%;
  height: 27rem;
  background-image: url(../../src/assets/img/footer-bg.jpg);
}
.footer-links-container {
  width: 40%;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
}
.dc-comics-links {
  display: flex;
  flex-direction: column;
  margin-top: 30px;
  line-height: 1.7em;
  margin-right: 10px;
  a {
    text-decoration: none;
    color: grey;
  }
}
.title-links {
  color: white;
  font-size: 18px;
  font-weight: bold;
}
.shop-links {
  margin-top: -60px;
}
.footer-container {
    position: relative;
}
.dc-logo-background {
    width: 530px;
    position: absolute;
    top: -120px;
    right: 0;
}
</style>