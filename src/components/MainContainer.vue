<template>
   <main>
        <JumbotronPlanning />
        <our-services :services="services"/>
        <JumbotronGrow />
        <Portfolio />
        <PriceList />
        <blog :posts="posts" />
        <testimonial :testimonials="testimonials" :sponsor="sponsor"/>
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
import testimonial from './Testimonial.vue'
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
    testimonial,
    SubscribeUserEmail,
  },
  data() {
    return {
      services: [ //SERVICES DATA
        {
          id: 0,
          image: 'Group-247',
          title: 'Data Analysis',
          paragraph: 'When, while the lovely valley teems with vapour around meand the meriadian sun strikes the upper'
        },
        {
          id: 1,
          image: 'Group-567',
          title: 'SEO Optimization',
          paragraph: 'When, while the lovely valley teems with vapour around meand the meriadian sun strikes the upper'
        },
        {
          id: 2,
          image:'Group-538',
          title: 'Security Data',
          paragraph: 'When, while the lovely valley teems with vapour around meand the meriadian sun strikes the upper'
        },
        {
          id: 3,
          image:'Group-566',
          title: 'Branding Strategy',
          paragraph: 'When, while the lovely valley teems with vapour around meand the meriadian sun strikes the upper'
        }     
      ],
      posts: [ // BLOG DATA
        {
          date: 'April 21, 2019',
          author: 'Paul',
          title: 'Clearing Corporations get SEBI nod to invest in overnight funds',
          paragraph: 'When, while the lovely valley teems with vapour around meand the meriadian sun strikes the upper'
        },
        {
          date: 'April 21, 2019',
          author: 'Paul',
          title: 'Shabnam Dhillion, wife of RSSB chief Gurinder Dhillon, passes away in London',
          paragraph: 'When, while the lovely valley teems with vapour around meand the meriadian sun strikes the upper'
        },
      ],
      testimonials: [  //TESTIMONIALS DATA
        {
          id: 0,
          photo: 'szabo-viktor-1266895-unsplash-1024x1024',
          vote_average: 3,
          review: 'When, while lovely valley teems with vapour around meand meridian sun strikes the upper impenetrable foliage of my trees, and but a thousand.',
          name:'Michkel Anegl',
          role: 'Marketing Management',
        },
        {
          id: 1,
          photo: 'philipe-cavalcante-539505-unsplash-1024x1024',
          vote_average: 3,
          review: 'When, while lovely valley teems with vapour around meand meridian sun strikes the upper impenetrable foliage of my trees, and but a thousand.',
          name:'Michkel Anegl',
          role: 'Marketing Management',
        },
        {
          id: 2,
          photo: 'fabio-spinelli-695744-unsplash-1024x1024',
          vote_average: 3,
          review: 'When, while lovely valley teems with vapour around meand meridian sun strikes the upper impenetrable foliage of my trees, and but a thousand.',
          name:'Michkel Anegl',
          role: 'Marketing Management',
        }
      ],
      sponsor: [
        'client-1-1',
        'clienty-2',
        'clienty-4',
        'client-5',
        'clienty-3',
      ],
    }
  },
}
</script>

<style lang="scss" scoped>

</style>