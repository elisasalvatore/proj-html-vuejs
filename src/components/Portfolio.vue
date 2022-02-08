<template>
    <div>
        <div class="section-container">
            <div class="section-top">
                <div class="text">
                    <div class="section-name">Portfolio</div>
                    <div class="section-title"><b>Titolo</b> Sezione</div>
                </div>

                <div class="arrows-slider">
                    FRECCE
                </div>
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