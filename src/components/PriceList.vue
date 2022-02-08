<template>
    <div>
        PRICE LIST
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';

div {
    height: 200px;
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