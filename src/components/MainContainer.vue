<template>
   <main>
        <JumbotronPlanning />
        <OurServices />
        <JumbotronGrow />
        <Portfolio />
        <PriceList />
        <Blog />
        <Testimonial />
        <SubscribeUserEmail />
   </main>
</template>

<script>
import JumbotronPlanning from './JumbotronPlanning.vue'
import OurServices from './OurServices.vue'
import JumbotronGrow from './JumbotronGrow.vue'
import Portfolio from './Portfolio.vue'
import PriceList from './PriceList.vue'
import Blog from './Blog.vue'
import Testimonial from './Testimonial.vue'
import SubscribeUserEmail from './SubscribeUserEmail.vue'

export default {
  name: 'MainContainer',
  components: {
    JumbotronPlanning,
    OurServices,
    JumbotronGrow,
    Portfolio,
    PriceList,
    Blog,
    Testimonial,
    SubscribeUserEmail,
  }
}
</script>