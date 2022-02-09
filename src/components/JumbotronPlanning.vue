<template>
    <div class="container-jumbo blue-gradient">
      <div class="jumbo-box">
        <div class="jumbo-title"><b>Business Planning</b> Digital Technology <b>Modern Solution !</b></div>
        <p class="jumbo-paragraph">When, while the lovely valley teems with vapour around meand the meridian sun strikes the upper surface.</p>

        <div class="container-buttons">
          <button>MEDIUM</button>
          <button>MEDIUM</button>
        </div>
      </div>

      <div class="jumbo-box">
        <img src="@/assets/images/header.png" alt="">
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

.jumbo-box {
  width: 500px;
  height: 450px;

  .jumbo-paragraph {
    width: 300px;
  }
}

</style>

