<script>
//Header component's
import HeaderNavbar from './components/HeaderNavbar.vue'
import HeaderJumbo from './components/HeaderJumbo.vue'

//Main component's
import MainService from './components/MainService.vue'
import MainAboutUs from './components/MainAboutUs.vue'
import MainDeliverCare from './components/MainDeliverCare.vue'
import MainProject from './components/MainProject.vue'
import MainTestimonial from './components/MainTestimonial.vue'
import MainBlog from './components/MainBlog.vue'

export default {
  name: 'App',
  components: {
    HeaderNavbar,
    HeaderJumbo,
    MainService,
    MainAboutUs,
    MainDeliverCare,
    MainProject,
    MainTestimonial,
    MainBlog
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
    <MainProject />
    <MainTestimonial />
    <MainBlog />
  </main>
</template>


<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;

main {
  background-color: $main-blue-color;
}
</style>