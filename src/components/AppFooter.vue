<script>
export default {
  name: 'AppFooter'
}
</script>

<template>
  <footer>
    <div class="footer-top">
      <div class="footer-resources">
        <div class="dc-shop">
          <div class="dc-comics-list">
            <h3>DC COMICS</h3>
            <ul>
              <li>Characters</li>
              <li>Comics</li>
              <li>Movies</li>
              <li>TV</li>
              <li>Games</li>
              <li>Videos</li>
              <li>News</li>
            </ul>
          </div>
          <div class="shop">
            <h3>SHOPS</h3>
            <ul>
              <li>Shop DC</li>
              <li>Shop DC Collectibles</li>
            </ul>
          </div>
        </div>
        <div class="dc">
          <div class="dc-list">
            <h3>DC</h3>
            <ul>
              <li>Terms Of Use</li>
              <li>Privacy policy (New)</li>
              <li>Ad Choices</li>
              <li>Advertising</li>
              <li>Jobs</li>
              <li>Subscriptions</li>
              <li>Talent Workshops</li>
              <li>CPSC Certificates</li>
              <li>Ratings</li>
              <li>Shop Help</li>
              <li>Contact Us</li>
            </ul>
          </div>
        </div>
        <div class="sites">
          <div class="sites-list">
            <h3>SITES</h3>
            <ul>
              <li>DC</li>
              <li>MAD Magazines</li>
              <li>DC Kids</li>
              <li>DC Universe</li>
              <li>DC Power Visa</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="footer-logo-img">
        <img src="../assets/img/dc-logo-bg.png" alt="">
      </div>
    </div>
    <div class="footer-bottom">
      <div class="sign-up">
        <a href="">SIGN-UP NOW!</a>
      </div>
      <div class="socials">
        <a href="">FOLLOW US</a>
        <div class="facebook">
          <img src="../assets/img/footer-facebook.png" alt="">
        </div>
        <div class="twitter">
          <img src="../assets/img/footer-twitter.png" alt="">
        </div>
        <div class="youtube">
          <img src="../assets/img/footer-youtube.png" alt="">
        </div>
        <div class="pinterest">
          <img src="../assets/img/footer-pinterest.png" alt="">
        </div>
        <div class="location">
          <img src="../assets/img/footer-periscope.png" alt="">
        </div>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
.footer-top {
  height: 400px;
  background-image: url(../assets/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  color: #929292;
  font-size: 12px;
  padding: 2rem 5rem;

  .footer-resources {
    display: flex;

    &>div {
      margin-right: 1.5rem;

      li {
        line-height: 1.5rem;
      }
    }
  }

  h3 {
    color: #fff;
    margin: .75rem 0;
    font-size: 18px;
  }

  .footer-logo-img {
    img {
      position: absolute;
      right: 10rem;
      top: -6rem;
      z-index: 1;
    }
  }
}

.footer-bottom {
  height: 100px;
  background-color: #303030;
  position: relative;
  z-index: 110;
  padding: 2rem 5rem;
  display: flex;
  justify-content: space-between;
  align-items: center;

  .sign-up {
    a {
      color: #fff;
      padding: .85rem;
      border: 3px solid #0282f9;
    }
  }

  .socials {
    display: flex;
    align-items: center;

    a {
      color: #0282f9;
      font-weight: bold;
      margin-right: 2rem;
    }

    &>div {
      margin-right: 1rem;
    }
  }

}
</style>