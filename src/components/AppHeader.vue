<script>
export default {
  name: 'AppHeader',
  data() {
    return {
      links: [
        {
          text: 'CHARACTERS',
          url: '#',
          current: false
        },
        {
          text: 'COMICS',
          url: '#',
          current: true
        },
        {
          text: 'MOVIES',
          url: '#',
          current: false
        },
        {
          text: 'TV',
          url: '#',
          current: false
        },
        {
          text: 'GAMES',
          url: '#',
          current: false
        },
        {
          text: 'COLLECTIBLES',
          url: '#',
          current: false
        },
        {
          text: 'VIDEOS',
          url: '#',
          current: false
        },
        {
          text: 'FANS',
          url: '#',
          current: false
        },
        {
          text: 'NEWS',
          url: '#',
          current: false
        },
        {
          text: 'SHOP',
          url: '#',
          current: false
        }
      ]
    }
  }
}
</script>

<template>
  <header>
    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="">
    </div>
    <nav>
      <ul>
        <li v-for="link in links" :class="link.current ? 'active' : ''"><a :href="link.url">{{ link.text }}</a></li>
      </ul>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
header {
  height: 100px;
  width: 100%;
  display: flex;
  justify-content: space-between;
  padding: 0 6rem;

  .logo {
    height: 100%;
    display: flex;
    align-items: center;

    img {
      height: 75%;
    }
  }

  nav {

    ul {
      display: flex;
      height: 100%;

      li {
        margin: 0 1rem;
        font-size: 13px;
        font-weight: bold;
        display: flex;
        align-items: center;

        a {
          color: rgb(98, 98, 98);
        }
      }
    }
  }

  .active {
    border-bottom: 5px solid #0282f9;

    a {
      color: #0282f9;
    }
  }
}
</style>