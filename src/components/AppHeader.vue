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
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.active {
  border-bottom: 5px solid $primary;

  a {
    color: $primary;
  }
}

header {
  width: 100%;
  @include flex-between;

  .logo {
    height: 100%;
    @include flex-align-center;

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
        @include flex-align-center;

        a {
          color: $grey;
        }
      }
    }
  }


}
</style>