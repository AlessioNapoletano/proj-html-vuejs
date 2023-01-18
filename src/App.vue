<script>
import HeaderNavbar from './components/HeaderNavbar.vue'

export default {
  name: 'App',
  components: {
    HeaderNavbar
  }
}
</script>

<template>
  <header>
    <HeaderNavbar />
  </header>
</template>


<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;
</style>