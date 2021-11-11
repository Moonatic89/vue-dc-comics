<template>
  <div class="siteHeader">
    <nav>
      <div class="logo">
        <img src="../assets/dc-logo.png" alt="" />
      </div>
      <ul>
        <li>CHARACTERS</li>
        <li class="bottomLine">COMICS</li>
        <li>MOVIES</li>
        <li>TV</li>
        <li>GAMES</li>
        <li>COLLECTIBLES</li>
        <li>VIDEOS</li>
        <li>FANS</li>
        <li>NEWS</li>
        <li>SHOP</li>
      </ul>
    </nav>
  </div>
</template>

<script>
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
@import "../assets/scss/variables.scss";
.siteHeader {
  height: 118px;

  nav {
    margin: auto;
    width: 70%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  ul {
    list-style: none;
    display: flex;
  }

  li {
    padding: 0 0.7rem;
    line-height: 118px;
  }
  .bottomLine {
    border-bottom: 2px solid blue;
  }
}
</style>
