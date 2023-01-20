<script>
//Header components
import HeaderNavbar from './components/HeaderNavbar.vue'
import HeaderJumbo from './components/HeaderJumbo.vue'

//Main components
import MainService from './components/MainService.vue'
import MainAboutUs from './components/MainAboutUs.vue'
import MainDeliverCare from './components/MainDeliverCare.vue'
import MainProject from './components/MainProject.vue'
import MainTestimonial from './components/MainTestimonial.vue'
import MainBlog from './components/MainBlog.vue'

//Footer components
import FooterGetStarted from './components/FooterGetStarted.vue'
import FooterNav from './components/FooterNav.vue'
import EndFooter from './components/EndFooter.vue'

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
    MainBlog,
    FooterGetStarted,
    FooterNav,
    EndFooter
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

  <footer>
    <FooterGetStarted />
    <FooterNav />
    <EndFooter />
  </footer>
</template>


<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;

main {
  background-color: $main-blue-color;
}

footer {
  background-color: $main-blue-color;
}
</style>