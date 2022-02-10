<template>
     <div class="section-container">
        <div class="section-name">Testimonial</div>
        <div class="section-title"><b>What</b> People Say</div>
        <p>When, while the lovely valley teems with vapour around meand the meriand sun strikes the upper surface.</p>

        <div class="testimonials-container" >
            <div class="testimonial-box" v-for="testimonial in testimonials" :key="testimonial.id">
               <img :src="require(`../assets/images/${testimonial.photo}.png`)">
               <div class="testimonial-vote">{{testimonial.vote_average}}</div>
               <div class="testimonial-review">{{testimonial.review}}</div>
               <div class="testimonial-name">{{testimonial.name}}</div>
               <div class="testimonial-role">{{testimonial.role}}</div>

            </div>
        </div>
    </div>
</template>

<script>
export default ({
    name: 'Testimonial',
    props: {
        testimonials: Array,
    }
})
</script>

<style lang="scss" scoped>
@import '@/style/sectionsHeading.scss';

.section-container {
    background-color: #fff;
    border: 2px solid red;

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
}
</style>
