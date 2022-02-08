<template>
    <div class="container-jumbo blue-gradient">
        <div class="jumbo-box">
         IMMAGINE
        </div>

        <div class="jumbo-box">
            <div>TITOLO</div>
            <p>Testo azzurro</p>

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

.container-jumbo {
  height: 60vh;

    .jumbo-box {
        height: 300px;
        width: 300px;
    }
}
</style>
