<script>
export default {
  name: 'ComicCard',
  props: {
    details: Object
  }
}
</script>

<template>
  <div class="card">
    <img :src="details.thumb" alt="">
    <p>{{ details.series }}</p>
    <p>{{ details.price }}</p>
    <p>{{ details.type }}</p>
  </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

.card {
  width: calc((100% / 6) - 2rem);
  margin: 0 1rem;

  img {
    width: 100%;
    height: 65%;
    object-fit: cover;
    object-position: top;
  }
}
</style>