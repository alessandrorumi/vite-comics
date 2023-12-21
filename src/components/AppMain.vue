<script>
export default {
  name: 'AppMain'
}
</script>

<template>
  <main>
    <h3>Content Goes Here</h3>
  </main>
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
main {
  height: 100px;
  background-color: #000;
  color: #fff;
}

.shop {
  height: 150px;
  background-color: #0282f9;
  display: flex;
  align-items: center;
  justify-content: center;
  color: #fff;

  &>div {
    display: flex;
    align-items: center;
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