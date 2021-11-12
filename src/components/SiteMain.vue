<template>
  <div class="siteMain">
    <div class="content">
      <!-- Here goes the grid -->
      <div class="row">
        <div>
        <Card v-for="card in cards" v-bind:thumb >

        </div>
      </div>

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
import Card from "./components/Card.vue";

export default {
  name: "SiteMain",
  components: {
    Card,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
.siteMain {
  position: relative;
  z-index: 1;
  height: 236px;
  background-color: black;

  .content {
    height: 118px;
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
