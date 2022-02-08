<template>
  <div id="app">
    <Header />
    <MainContainer />
    <Footer />
  </div>
</template>

<script>
import Footer from './components/Footer.vue'
import Header from './components/Header.vue'
import MainContainer from './components/MainContainer.vue'

export default {
  name: 'App',
  components: {
    Header,
    MainContainer,
    Footer,
  }
}
</script>

<style lang="scss">
@import './style/main.scss';
@import './style/variables.scss';
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400;500;700&display=swap');
</style>
