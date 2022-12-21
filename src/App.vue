<script>
import Header from './components/Header.vue'
import HomeMain from './components/HomeMain.vue'
import Footer from './components/Footer.vue'

export default {
  components: {
    Header,
    HomeMain,
    Footer
  },
};
</script>

<template>
  <Header />
  <HomeMain />
  <Footer />
</template>

<style lang="scss" scoped>
@use './styles/general.scss' as *;
@use './styles/partials/mixins' as *;
@use './styles/partials/variables' as *;
</style>