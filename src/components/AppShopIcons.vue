<script>
export default {
  name: 'AppShopIcons'
}
</script>

<template>
  <section>
    <div class="shop">
      <div class="digital-comics">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
        DIGITAL COMICS
      </div>
      <div class="merchandise">
        <img src="../assets/img/buy-comics-merchandise.png" alt="">
        DC MERCHANDISE
      </div>
      <div class="sub">
        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
        SUBSCRIPTION
      </div>
      <div class="shop-locator">
        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
        COMIC SHOP LOCATOR
      </div>
      <div class="visa">
        <img src="../assets/img/buy-dc-power-visa.svg" alt="">
        DC POWER VISA
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.shop {
  height: 150px;
  background-color: $primary;
  @include flex-align-center;
  justify-content: center;
  color: $secondary;
  position: relative;
  z-index: 100;

  &>div {
    @include flex-align-center;
    height: 100%;
    margin: 1.75rem;

    img {
      height: 40%;
      margin-right: .5rem;
    }
  }

  .visa {
    img {
      width: 35%;
    }
  }
}
</style>