<template>
    <div class="section-container">
        <div class="section-name">Price List</div>
        <div class="section-title"><b>Titolo</b> Sezione</div>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Explicabo odio unde dolores similique assumenda cupiditate aspernatur nobis</p>

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
    border: 2px solid red;
    color: white;
    background-color: $brg-blue;
    background-image:
    // doppio gradiente: sopra blu (a sx chiaro a de scuro) sotto bianco
    linear-gradient(
        $brg-blue 50%,
        #fff 50%,
    );
}
</style>