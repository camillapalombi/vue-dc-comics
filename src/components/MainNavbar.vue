<template>
  <nav>
      <div class="container nav-container">
          <div class="nav-item">
              <img src="../../src/assets/img/buy-comics-digital-comics.png" alt="Digital Comics">
              <div>DIGITAL COMICS</div>
          </div>
          <div class="nav-item">
              <img src="../../src/assets/img/buy-comics-merchandise.png" alt="Digital Comics">
              <div>DC MERCHANDISE</div>
          </div>
          <div class="nav-item">
              <img src="../../src/assets/img/buy-comics-subscriptions.png" alt="Digital Comics">
              <div>SUBSCRIPTION</div>
          </div>
          <div class="nav-item">
              <img class="img-locator" src="../../src/assets/img/buy-comics-shop-locator.png" alt="Digital Comics">
              <div>COMIC SHOP LOCATOR</div>
          </div>
          <div class="nav-item">
              <img src="../../src/assets/img/buy-dc-power-visa.svg" alt="Digital Comics">
              <div>DC POWER VISA</div>
          </div>

      </div>
  </nav>
</template>

<script>
export default {
name: 'MainNavbar',
}
</script>

<style scoped lang="scss">
nav {
    z-index: 20;
    background-color: #0282f9;
    color: white;
    font-size: 12px;
    .nav-container {
        justify-content: space-between;
        align-items: center;
        height: 9rem;
    }
}
.nav-item {
    display: flex;
    align-items: center;
    cursor: pointer;
}
img {
    width: 40px;
    margin-right: 15px
}
.img-locator {
    width: 30px;
}
</style>