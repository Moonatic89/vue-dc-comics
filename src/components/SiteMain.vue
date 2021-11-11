<template>
  <div class="siteMain">
    <div class="content">
      <span> --&#62; Content goes here &#60;-- </span>
    </div>
    <div class="grid">
      <div class="row">
        <ul>
          <li>DIGITAL COMICS</li>
          <li>DC MERCHANDISE</li>
          <li>SUBSCRIPTION</li>
          <li>COMIC SHOP LOCATOR</li>
          <li>DC POWER VISA</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
.siteMain {
  height: 118px;
  background-color: black;

  .content {
    margin: auto;
    width: 70%;

    span {
      color: white;
      font-size: 2rem;
      line-height: 118px;
    }
  }

  .grid {
    height: 118px;
    background-color: cornflowerblue;
  }
  ul {
    height: 118px;
    margin: auto;
    list-style: none;
    width: 70%;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  li {
    padding: 0 0.5rem;
    font-size: 1rem;
    color: white;
  }
}
</style>
