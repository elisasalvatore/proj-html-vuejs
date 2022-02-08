<template>
    <div class="container-jumbo blue-gradient">
      <div class="jumbo-box">
        <div>TITOLO</div>
        <p>Testo azzurro</p>

        <div class="container-buttons">
          <button>BOTTONE</button>
          <button>BOTTONE</button>
        </div>
      </div>

      <div class="jumbo-box">
        IMMAGINE
      </div>
    </div>
</template>

<script>

export default ({
  name: 'JumbotronPlanning',

})
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
@import '@/style/jumbotron.scss';

.container-jumbo {
  height: 80vh;

  .jumbo-box {
    height: 400px;
    width: 400px;
  }
}

</style>

