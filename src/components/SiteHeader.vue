<template>
  <div class="">
    <header id="site_header">
      <div class="logo">
        <img src="../assets/dc-logo.png" alt="" width="60">
      </div>
      <ul>
        <li>CHARACTERS</li>
        <li class="list_active">COMICS</li>
        <li>MOVIES</li>
        <li>TV</li>
        <li>GAMES</li>
        <li>COLLECTIBLES</li>
        <li>VIDEOS</li>
        <li>FANS</li>
        <li>NEWS</li>
        <li>SHOP</li>
      </ul>
    </header>

  </div>
</template>

<script>
</script>

<style lang="scss">
@import '../assets/scss/variables.scss';
#site_header{
  display: flex;
  justify-content: space-between;
  align-items: end;
  padding-top: 2rem;
.logo {
  padding-bottom: 1rem;
}
ul {
  display: flex;
  list-style: none;
  li {
    padding: 0 1rem;
  }
  .list_active {
      color: $color_primary;
      &::after {
        content: "";
        display: block;
        width: 50px;
        height: 5px;
        background-color: $color_primary;
        margin: auto;
        margin-top: 2rem;
      }
    }

}
}
</style>
