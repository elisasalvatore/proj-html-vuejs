<template>
  <div id="app">
    <Header :navItems="navItems"/>
    <main-container />
    <Footer :resources="resources" :links="links" :contacts="contacts"/>
  </div>
</template>

<script>
import Footer from './components/Footer.vue'
import Header from './components/Header.vue'
import MainContainer from './components/MainContainer.vue'

export default {
  name: 'App',
  data() {
    return {
      navItems: [ // NAV MENU
        'Home',
        'About',
        'Services',
        'Blog',
        'Contact',
        'Portfolio',
      ],
      links: [ // FOOTER 
        'Services',
        'Contact',
        'Blog'
      ],
      resources: [
        'Art Design',
        'Computer',
        'IT News',
        'Networking',
        'Web Security'
      ],
      contacts: [
        {
          type: 'Address',
          value: 'Patricia C. Amedee 4401 Waldeck Street Grapevine Nashville, Tx 76051'
        },
         {
          type: 'Phone',
          value: '+39(0) 101 0000 888'
        },
         {
          type: 'Email',
          value: 'info@yourdomain.com'
        }
      ],
    }
  },
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
