<template>
  <header>
    <div class="logo">
      <img src="@/assets/images/white-logo-2.png" alt="logo">
    </div>

    <div class="nav-menu">
      NAV
      <button>Sign In</button>
    </div>


  </header>
</template>

<script>
export default {
  name: 'Header',
  
}
</script>

<style scoped lang="scss">
@import '@/style/variables.scss';

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 80px;
  padding: 0 80px;
  background-color: $brg-blue; 
  color: #fff;

  .logo > img {
   width: 100px;
   height: 40px;
  }
}

</style>
