<script>
export default {
  name: 'AppMain'
}
</script>

<template>
  <main>
    <h3>Content Goes Here</h3>
  </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

main {
  background-color: #000;
  color: $secondary;
  @include flex-align-center;
}
</style>