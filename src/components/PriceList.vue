<template>
    <div class="section-container">
        <div class="section-name">Price List</div>
        <div class="section-title"><b>Titolo</b> Sezione</div>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo odio unde dolores similique assumenda cupiditate aspernatur nobis</p>

        <div class="price-cards">
            <!-- TODO RENDERE DINAMICO V-FOR ?-->
            <div class="card">
                <h1 class="card-title">Title</h1>
                <div class="card-subtitle">Subtitle</div>
                <div class="card-dollar-sign">$</div>
                <h1 class="card-price">40</h1>
                <div class="card-month">Per Month</div>
                <div class="card-details">
                    <div class="detail"><b>Creative</b> Design Enabled</div>
                    <div class="detail"><b>Vibrant</b> Color Usage</div>
                    <div class="detail"><b>Eye</b> Catching Design</div>
                    <div class="detail"><b>Extreme</b> Typography</div>
                    <div class="detail"><b>Exceptional</b> Design</div>
                </div>
                <button>LARGE</button>
            </div>
            <div class="card"></div>
            <div class="card"></div>
            
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
    height: 80vh;
    padding: 40px;
    border: 2px solid red;
    color: white;
    background-color: $brg-blue;
    background-image:
    // doppio gradiente: sopra blu (a sx chiaro a de scuro) sotto bianco
    linear-gradient(
        $brg-blue 50%,
        #fff 50%,
    );

    .price-cards {
        display: flex;
        justify-content: space-around;

        .card {
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            align-items: center;
            width: calc(100% / 3);
            min-width: 240px;
            max-width: 240px;
            height: 300px;
            border-radius: 20px;
            margin: 20px 10px;
            padding: 20px 0;
            background-color:cadetblue ;

            .card-details {
                font-size: 12px;
                padding: 20px 10px;
                font-weight: lighter;

                .detail {
                    margin: 5px 0;

                }
            }
        }
    }
}
</style>