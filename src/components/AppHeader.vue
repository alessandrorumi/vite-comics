<script>
export default {
  name: 'AppHeader'
}
</script>

<template>
  <header>
    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="">
    </div>
    <nav>
      <ul>
        <li><a href="">CHARACTERS</a></li>
        <li><a href="">COMICS</a></li>
        <li><a href="">MOVIES</a></li>
        <li><a href="">TV</a></li>
        <li><a href="">GAMES</a></li>
        <li><a href="">COLLECTIBLES</a></li>
        <li><a href="">VIDEOS</a></li>
        <li><a href="">FANS</a></li>
        <li><a href="">NEWS</a></li>
        <li><a href="">SHOP</a></li>
      </ul>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
header {
  height: 100px;
  width: 100%;
  display: flex;
  justify-content: space-evenly;

  .logo {
    height: 100%;
    display: flex;
    align-items: center;

    img {
      height: 75%;
    }
  }

  nav {
    display: flex;
    align-items: center;

    ul {
      display: flex;

      li {
        margin: 0 .75rem;
      }
    }
  }

}
</style>