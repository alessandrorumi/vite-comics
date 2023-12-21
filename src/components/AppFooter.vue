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
              <li><a href="">Characters</a></li>
              <li><a href="">Comics</a></li>
              <li><a href="">Movies</a></li>
              <li><a href="">TV</a></li>
              <li><a href="">Games</a></li>
              <li><a href="">Videos</a></li>
              <li><a href="">News</a></li>
            </ul>
          </div>
          <div class="shop">
            <h3>SHOPS</h3>
            <ul>
              <li><a href="">Shop DC</a></li>
              <li><a href="">Shop DC Collectibles</a></li>
            </ul>
          </div>
        </div>
        <div class="dc">
          <div class="dc-list">
            <h3>DC</h3>
            <ul>
              <li><a href="">Terms Of Use</a></li>
              <li><a href="">Privacy policy (New)</a></li>
              <li><a href="">Ad Choices</a></li>
              <li><a href="">Advertising</a></li>
              <li><a href="">Jobs</a></li>
              <li><a href="">Subscriptions</a></li>
              <li><a href="">Talent Workshops</a></li>
              <li><a href="">CPSC Certificates</a></li>
              <li><a href="">Ratings</a></li>
              <li><a href="">Shop Help</a></li>
              <li><a href="">Contact Us</a></li>
            </ul>
          </div>
        </div>
        <div class="sites">
          <div class="sites-list">
            <h3>SITES</h3>
            <ul>
              <li><a href="">DC</a></li>
              <li><a href="">MAD Magazines</a></li>
              <li><a href="">DC Kids</a></li>
              <li><a href="">DC Universe</a></li>
              <li><a href="">DC Power Visa</a></li>
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
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.footer-top {
  height: 400px;
  background-image: url(../assets/img/footer-bg.jpg);
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  font-size: .75rem;
  padding: 2rem 6rem;

  .footer-resources {
    display: flex;

    &>div {
      margin-right: 1.5rem;

      li {
        line-height: 1.5rem;

        a {
          color: #929292;
        }
      }
    }
  }

  h3 {
    color: #fff;
    margin: .75rem 0;
    font-size: 1.25rem;
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
  @include space-between;
  align-items: center;
  padding: 0 6rem;

  .sign-up {
    a {
      color: #fff;
      padding: .85rem;
      border: 3px solid $primary;
    }
  }

  .socials {
    @include vertical-flex;

    a {
      color: $primary;
      margin-right: 2rem;
    }

    &>div {
      margin-right: 1rem;
    }
  }

}
</style>