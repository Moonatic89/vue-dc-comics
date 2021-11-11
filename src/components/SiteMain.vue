<template>
  <div class="siteMain">
    <div class="content">
      <span> --&#62; Content goes here &#60;-- </span>
    </div>
    <div class="grid">
      <div class="row">
        <ul>
          <li>
            <img src="../assets/buy-comics-digital-comics.png" alt="" />
            DIGITAL COMICS
          </li>
          <li>
            <img src="../assets/buy-comics-merchandise.png" alt="" />
            DC MERCHANDISE
          </li>
          <li>
            <img src="../assets/buy-comics-subscriptions.png" alt="" />
            SUBSCRIPTION
          </li>
          <li>
            <img src="../assets/buy-comics-shop-locator.png" alt="" />
            COMIC SHOP LOCATOR
          </li>
          <li>
            <img src="../assets/buy-dc-power-visa.svg" alt="" />
            DC POWER VISA
          </li>
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

    ul {
      height: 118px;
      margin: auto;
      width: 70%;
      list-style: none;
      display: flex;
      justify-content: space-between;
      align-items: center;

      img {
        height: 50px;
        max-width: 50px;
      }

      li {
        display: flex;
        align-items: center;
        padding: 0 0.5rem;
        font-size: 1rem;
        color: white;
      }
    }
  }
}
</style>
