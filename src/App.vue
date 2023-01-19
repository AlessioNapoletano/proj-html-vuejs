<script>
//Header component's
import HeaderNavbar from './components/HeaderNavbar.vue'
import HeaderJumbo from './components/HeaderJumbo.vue'

//Main component's
import MainService from './components/MainService.vue'
import MainAboutUs from './components/MainAboutUs.vue'
import MainDeliverCare from './components/MainDeliverCare.vue'

export default {
  name: 'App',
  components: {
    HeaderNavbar,
    HeaderJumbo,
    MainService,
    MainAboutUs,
    MainDeliverCare
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
    <MainAboutUs />
    <MainDeliverCare />
  </main>
</template>


<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;

main {
  background-color: $main-blue-color;
}
</style>