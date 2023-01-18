<script>
//Header component's
import HeaderNavbar from './components/HeaderNavbar.vue'
import HeaderJumbo from './components/HeaderJumbo.vue'

//Main component's
import MainService from './components/MainService.vue'

export default {
  name: 'App',
  components: {
    HeaderNavbar,
    HeaderJumbo,
    MainService
  }
}
</script>

<template>
  <header>
    <HeaderNavbar />
    <HeaderJumbo />
  </header>

  <main>
    <MainService />
  </main>
</template>


<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;
</style>