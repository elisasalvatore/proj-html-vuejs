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
             <button>BOTTONE</button>
             <button>BOTTONE</button>
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
@import '@/style/variables.scss';
@import '@/style/jumbotron.scss';

.jumbo-box {
    > p {
        font-size: 12px;
        color: #fff;
    }

    .jumbo-title {
        margin-top: 20px;
    }

    button {
        margin-top: 20px;
    }
   
}

.box-images{
    width: 300px;
    height: 300px;
    position: relative;

    .man {
        position: absolute;
        left: 30%;
        width: 300px;
    }

    .graphic {
        position: absolute;
        left: 20%;
        bottom: 20%;
        width: 300px;   
    }
}

.box-text {
    width: 400px;
}
</style>
