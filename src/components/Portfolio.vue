<template>
    <div>
        <div class="section-container">
            <div class="section-top">
                <span class="text">
                    <div class="section-name">Portfolio</div>
                    <span class="section-title"><b>latest</b> work</span>
                </span>

                <span class="arrows-slider">
                    <span>&#x2190;</span>
                    <span>&#x2192;</span>
                </span>
            </div>

            <div class="section-down">
                <div class="slider">
                    SLIDER
                </div>
                <div class="slider-points">
                    punti slider
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
@import '@/style/sectionsHeading.scss';


.section-container {
    height: 60vh;
    text-align: start;
    background-color: #fff;

    .section-top {
        display: flex;
        justify-content: space-between;
        align-items: flex-end;
        padding: 0 60px;

        .arrows-slider  > span {
            height: 40px;
            line-height: 40px;
            margin: 10px;
            padding: 6px 8px;
            font-size: 20px;
            color: $light-pink;
            border: 1px solid $light-pink;
            border-radius: 50px;
            
            &:hover {
                cursor: pointer;
                background-color: $light-pink;
                color: #fff;
            }
        }
    }

    .section-down {
        background-color: brown;

        .slider {
            // DISPLAY FLEX
            padding: 40px 0;
        }

        .slider-points {
            // DISPLAY FLEX
            padding-bottom: 20px;
        }
    }
}
</style>