<template>
  <footer>
      <!--FOOTER TOP-->
    <div class="footer-top">

      <div class="container footer-container-top">

        <div class="footer-links-container">

          <div class="dc-comics-links">
            <div class="title-links">DC COMICS</div>
            <a href="#!" v-for="link1 in dcComicsLinks" :key="link1">{{link1.text}}</a>
          </div>

          <div class="dc-comics-links">
            <div class="title-links">DC</div>
            <a href="#!" v-for="link2 in dcLinks" :key="link2">{{ link2.text }}</a>
          </div>

          <div class="dc-comics-links">
            <div class="title-links">SITE</div>
            <a href="#!" v-for="link3 in siteLinks" :key="link3">{{ link3.text }}</a>
          </div>

          <div class="dc-comics-links shop-links">
            <div class="title-links">SHOP</div>
            <a href="#!" v-for="link4 in shopLinks" :key="link4">{{link4.text}}</a>
          </div>

        </div>

        <img class="dc-logo-background" src="../../src/assets/img/dc-logo-bg.png" alt="" />

      </div>
    </div>

    <!--FOOTER BOTTOM-->
    <div class="footer-bottom">

        <div class="container footer-container-bottom">

            <div class="btn-container">
                <button>SIGN-UP NOW!</button>
            </div>

            <div class="follow-container">
                <span>FOLLOW US</span>
                <img src="../../src/assets/img/footer-facebook.png" alt="facebook">
                <img src="../../src/assets/img/footer-twitter.png" alt="twitter">
                <img src="../../src/assets/img/footer-youtube.png" alt="youtube">
                <img src="../../src/assets/img/footer-pinterest.png" alt="pinterest">
                <img src="../../src/assets/img/footer-periscope.png" alt="periscope">
            </div>

        </div>

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
@import '../assets/style/partials/variables';

.footer-top {
  width: 100%;
  height: 27rem;
  background-image: url(../../src/assets/img/footer-bg.jpg);
  overflow: hidden;
    .footer-container-top {
      position: relative;
        .footer-links-container {
          width: 40%;
          display: flex;
          flex-wrap: wrap;
          justify-content: space-between;
            .dc-comics-links {
              display: flex;
              flex-direction: column;
              margin-top: 30px;
              line-height: 1.7em;
              margin-right: 10px;
                a {
                  text-decoration: none;
                  color: $textLightGrey;
                }
            }
        }
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
.dc-logo-background {
  width: 550px;
  position: absolute;
  overflow: hidden;
  top: -100px;
  right: 0;
}
.footer-bottom {
    height: 6rem;
    background-color: $footerBackground;
    position: relative;
    z-index: 10;
      .footer-container-bottom {
        height: 100%;
        display: flex;
        justify-content: space-between;
          .btn-container {
            height: 100%;
            display: flex;
            align-items: center;
              button {
                background-color: transparent;
                padding: .8em;
                color: white;
                font-weight: bold;
                font-size: 15px;
                border: none;
                border: 3px solid $activeColor;
                cursor: pointer;
              }
          }
      }
}

.follow-container {
    width: 35%;
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
      span {
        font-weight: bold;
        color: $activeColor;
        font-size: 18px;
      }
      img {
        cursor: pointer;
      }
}
</style>