<template>
     <div class="section-container">
        <div class="section-name">Testimonial</div>
        <div class="section-title"><b>What</b> People Say</div>
        <p>When, while the lovely valley teems with vapour around meand the meriand sun strikes the upper surface.</p>

        <div class="testimonials-container" >
            <div class="testimonial-box" v-for="testimonial in testimonials" :key="testimonial.id">
               <img :src="require(`../assets/images/${testimonial.photo}.png`)">
               <div class="testimonial-vote"></div><stars-rating :vote="testimonial.vote_average"/>
               <div class="testimonial-review">{{testimonial.review}}</div>
               <div class="testimonial-name">{{testimonial.name}}</div>
               <div class="testimonial-role">{{testimonial.role}}</div>
            </div>
        
        </div>

        <div class="sponsor-container">
            <div class="sponsor-box" v-for="(item, i) in sponsor" :key="i">
                <img :src="require(`../assets/images/${sponsor[i]}.png`)">
            </div>
        </div>
    </div>
</template>

<script>
import StarsRating from './StarsRating.vue'

export default ({
    name: 'Testimonial',
    components: {
        StarsRating,
    },
    props: {
        testimonials: Array,
        sponsor: Array,
    }
})
</script>

<style lang="scss" scoped>
@import '@/style/main.scss';
@import '@/style/sectionsHeading.scss';

.section-container {
    background-color: #fff;
    
    .testimonials-container {
        display: flex;
        justify-content: space-between;
        height: 300px;
        padding: 0 50px;
        
        .testimonial-box {
            width: calc(100% / 3);
            height: 225px;
            padding: 15px;
            // background-color: blueviolet;

            > img {
                width: 80px;
                height: 80px;
                border: 2px solid $dark-pink;
                border-radius: 50%;
            }
        
            .testimonial-vote {
                padding-top: 20px;
            }

            .testimonial-review {
                font-size: 10px;
                word-spacing: 0.5px;
                padding: 20px 0;
                color: $text-gray;
            }

            .testimonial-name {
                font-size: 12px;
                font-weight: 600;
            }

            .testimonial-role {
                padding: 10px 0;
                font-size: 11px;
                font-weight: 300;
            }
        }
    }

    .sponsor-container {
        display: flex;
        justify-content: space-around;
        align-items: center;
        padding: 20px 0;

        .sponsor-box {
            > img {
                width: 70px;
            }
        }

    }
}
</style>
