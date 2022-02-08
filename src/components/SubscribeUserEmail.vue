<template>
    <div>
        SUBSCRIBE EMAIL
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
    background-color: $brg-blue;
    background-image:
    // doppio gradiente: sopra blu (a sx chiaro a de scuro) sotto bianco
    linear-gradient(
        #fff 50%,
        $brg-blue 50%,
    );
}
</style>