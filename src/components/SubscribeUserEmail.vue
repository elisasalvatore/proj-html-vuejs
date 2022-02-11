<template>
    <div class="container">
        <div class="subscribe-box pink-gradient">
            <div class="subscribe-text">
                <h1>We Offer Awesome Services</h1>
                <p>When, while lovely valley teems with vapour around meand meridian sun strikes the upper surface.</p>
            </div>

            <div class="subscribe-input">
                <input type="text" placeholder="Enter your Email Address">
                <button class="bt-medium bg-blue-light-to-dark">Subscribe</button>  
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

.container {
    display:flex;
    justify-content: center;
    align-items: center;
    height: 200px;
    padding: 30px;
    background-color: $brg-blue;
    background-image:
    // doppio gradiente: sopra blu (a sx chiaro a de scuro) sotto bianco
    linear-gradient(
        #fff 50%,
        $brg-blue 50%,
    );

    .subscribe-box.pink-gradient {
        color: #fff;
            background-color: $dark-pink;
            background-image: linear-gradient(
                to left,
                $light-pink,
                $dark-pink, 
            );
    }

    .subscribe-box {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 900px;
        height: 60px;
        padding: 50px 25px;
        border-radius: 20px;
        
        .subscribe-text {
            width: 510px;

            p {
                font-size: 12px;
                font-weight: lighter;
                padding: 10px 0;
            }
        }

        .subscribe-input {
            display: flex;
            justify-content: end;
            align-items: center;
            padding: 4px;
            border-radius: 25px;
            background-color: #fff;

            input {
                width: 200px;
                border: none;
                padding: 10px;
                border-radius: 20px;
                color: #ccc;
            }

            button {
                width: 90px;
                margin: 0 5px;
            }
        }
    }
}
</style>