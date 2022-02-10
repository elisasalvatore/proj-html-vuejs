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

                <div class="arrow">
                    <div class="bg-pink-dark-to-light">&#8702;</div>
                </div>
            </div>
        </div>

        <div class="bt-service">
            <button class="bt-large bg-pink-dark-to-light shadow-pink">View All Services</button>  
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
    margin-bottom: 20px;

    .services-container {
        display: flex;
        justify-content: space-between;
        height: 300px;
        padding: 0 40px;
        
        .service-box {
            width: calc(100% / 4);
            padding: 20px;

            >img {
                width: 120px;
                height: 110px;
            }

            .service-title {
                margin: 20px 0;
                font-weight: 500;
            }

            .service-paragraph {
                padding: 0 10px;
                font-size: 11px;
                letter-spacing: 0.5px;
                color: $text-gray;
            }

            .arrow {
                display: none;
                cursor: pointer;

                > .bg-pink-dark-to-light {
                    margin: 20px auto;
                    position: relative;
                    top: 8%;
                    width: 50px;
                    height: 50px;
                    line-height: 50px;
                    border-radius: 50%;
                    background-color: $dark-pink;
                    font-size: 25px;
                    background-color: $dark-pink;
                    background-image: linear-gradient(
                        to left top,
                        $light-pink,
                        $dark-pink, 
                    );
                }
                
            }

            &:hover {
                color: #fff;
                background-color: $brg-blue;
                border-radius: 20px;
                
                > img {
                    width: 100px;
                    height: 90px;
                    padding: 9px;
                    background-color: #fff;
                    border-radius: 20px;
                }

                .service-paragraph {
                    color: #fff;
                }

                .arrow {
                    display: inline;
                }
                
            }
        }

    }

    .bt-service {
        display: flex;
        justify-content: center;
        align-items: center;
        margin: 20px 0;
    }
}
</style>