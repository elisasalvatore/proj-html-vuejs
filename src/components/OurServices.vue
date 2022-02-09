<template>
    <div class="section-container">
        <div class="section-name">Our Services</div>
        <div class="section-title"><b>What</b> We DO</div>
        <p>When, while the lovely valley teems with vapour around meand the</p>

        <div class="services-container">
            <div class="service-box" >
                <img src="@/assets/images/Group-247.png" alt="">
                <h4 class="service-title">Data Analysis</h4>
                <div class="service-paragraph">When, why the lovely valley teems with vapour around meand the meriadian sun strikes the upper</div>
            </div>

             <div class="service-box" >
                <img src="@/assets/images/Group-567.png" alt="">
                <h4 class="service-title">SEO Optimization</h4>
                <div class="service-paragraph">When, why the lovely valley teems with vapour around meand the meriadian sun strikes the upper</div>
            </div>

             <div class="service-box" >
                <img src="@/assets/images/Group-538.png" alt="">
                <h4 class="service-title">Security Data</h4>
                <div class="service-paragraph">When, why the lovely valley teems with vapour around meand the meriadian sun strikes the upper</div>
            </div>

             <div class="service-box" >
                <img src="@/assets/images/Group-566.png" alt="">
                <h4 class="service-title">Branding Strategy</h4>
                <div class="service-paragraph">When, why the lovely valley teems with vapour around meand the meriadian sun strikes the upper</div>
            </div>
        </div>

        <button>LARGE</button>
    </div>
</template>

<script>
export default {
    name: 'OurServices',
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
@import '@/style/sectionsHeading.scss';

.section-container {
    height: 80vh;
    background-color: #fff;

    .services-container {
        display: flex;
        justify-content: space-between;
        height: 300px;
        padding: 0 50px;
        
        .service-box {
            width: calc(100% / 4);
            padding: 40px;

            > img {
                width: 100px;
            }

            .service-title {
                margin: 20px 0;
            }

            .service-paragraph {
                font-size: 10px;
                padding: 0 40px;
                color: $text-gray;
            }
        }
    }
}
</style>