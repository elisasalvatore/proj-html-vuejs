<template>
    <div class="section-container">
        <div class="section-name">Our Services</div>
        <div class="section-title"><b>What</b> We DO</div>
        <p>When, while the lovely valley teems with vapour around meand the</p>

        <div class="services-container">
            <div class="service-box" v-for="service in services" :key="service.id">
                <img :src="require(`../assets/images/${service.image}.png`)">
                <div class="service-title">{{service.title}}</div>
                <div class="service-paragraph">{{service.paragraph}}</div>
            </div>
        </div>

        <div class="bt-service">
            <button>LARGE</button>  
        </div>
    </div>
</template>

<script>
export default {
    name: 'OurServices',
    props: {
        services: Array,
    },
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
@import '@/style/sectionsHeading.scss';

.section-container {
    background-color: #fff;

    .services-container {
        display: flex;
        justify-content: space-between;
        height: 300px;
        padding: 0 50px;
        
        .service-box {
            width: calc(100% / 4);
            padding: 40px;


                >img {
                    width: 120px;
                    height: 110px;
                }


            .service-title {
                margin: 20px 0;
                font-weight: 500;
            }

            .service-paragraph {
                font-size: 11px;
                letter-spacing: 0.5px;
                color: $text-gray;
            }
        }
    }
}
</style>