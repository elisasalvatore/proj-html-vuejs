<template>
    <div class="container-jumbo blue-gradient">
        <div class="jumbo-box box-images">
         <img class="graphic" src="@/assets/images/nemoodar.png" alt="">
         <img class="man" src="@/assets/images/men-data.png" alt="">
        </div>

        <div class="jumbo-box box-text">
            <p>Start Your Project</p>
            <div class="jumbo-title"><b>Grow Your Business</b> With Our Strategy</div>
            <p class="jumbo-paragraph">When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper surface. Of the impenetrable folliage of my trees, and but a few stray gleams steal into the inner sanctuary.</p>

            <div class="container-buttons">
             <button class="bt-medium bg-pink-dark-to-light">Try It Now</button>
             <button class="bt-medium bg-blue-light-to-dark">Explore More</button>
            </div>
        </div>
    </div>
</template>

<script>

export default ({
    name: 'JumbotronGrow',
})
</script>

<style lang="scss" scoped>
@import '@/style/jumbotron.scss';

.jumbo-box {
    
    > p {
        margin-bottom: 10px;
        font-size: 12px;
        color: #fff;
    }
}

.box-images{
    width: 300px;
    height: 300px;
    position: relative;

    .man {
        position: absolute;
        top: 20%;
        left: 20%;
        width: 280px;
    }

    .graphic {
        position: absolute;
        top: 15%;
        left: 15%;
        width: 280px;   
    }
}

.box-text {
    width: 400px;
}
</style>
