<template>
  <header>
    <div class="logo">
      <img src="@/assets/images/white-logo-2.png" alt="logo">
    </div>

    <div class="nav-menu">
      <ul>
        <li v-for="(item, i) in navItems" :key="i" :item="item">
          {{item}}
        </li>
      </ul>

      <button class="bt-header bg-blue-light-to-dark">Sign In</button>
    </div>

  </header>
</template>

<script>
export default {
  name: 'Header',
  props: {
    navItems: Array,
  }
}
</script>

<style scoped lang="scss">
@import '@/style/main.scss';
@import '@/style/variables.scss';

header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 80px;
  padding: 0 60px;
  background-color: $brg-blue; 
  color: #fff;

  .logo > img {
   width: 100px;
   height: 40px;
   cursor: pointer;
  }

  .nav-menu {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 480px;
    padding: 5px;

    ul {
      width: 350px;
      display: flex;
      justify-content: space-between;
      padding: 0 5px;

      li {
        list-style: none;
        font-size: 13px;
        font-weight: 400;
        color: #fff;
        cursor: pointer;

        &:hover {
          color: $light-pink;
          font-weight: bold;
        }
      }
    }
  }
}

</style>
