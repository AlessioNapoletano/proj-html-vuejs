<script>
import HeaderNavbar from './components/HeaderNavbar.vue'
import HeaderJumbo from './components/HeaderJumbo.vue'

export default {
  name: 'App',
  components: {
    HeaderNavbar,
    HeaderJumbo
  }
}
</script>

<template>
  <header>
    <HeaderNavbar />
    <HeaderJumbo />
  </header>
</template>


<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;
</style>