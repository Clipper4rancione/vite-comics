<script>
export default {
  name: "AppHeader",
};
</script>

<template>
  <header>
    <div class="h-wrapper">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="" />
      </div>
      <div class="nav-menu">
        <ul>
          <li><a href="">characters</a></li>
          <li><a href="">comics</a></li>
          <li><a href="">movies</a></li>
          <li><a href="">tv</a></li>
          <li><a href="">games</a></li>
          <li><a href="">collectibles</a></li>
          <li><a href="">videos</a></li>
          <li><a href="">fans</a></li>
          <li><a href="">news</a></li>
          <li><a href="">shop</a></li>
        </ul>
      </div>
    </div>
  </header>
</template>


<style lang="scss" scoped>
header {
  height: 110px;
  width: 100%;
  background-color: white;

  .h-wrapper {
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 100%;

    img {
      vertical-align: middle;
    }
  }

  ul {
    cursor: pointer;
    height: 100%;
    list-style: none;
    display: flex;

    a {
      padding: 15px;
      text-decoration: none;
      text-transform: uppercase;
      color: black;
      font-size: 0.92rem;
    }
  }
}
</style>