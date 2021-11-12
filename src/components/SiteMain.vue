<template>
  <div class="siteMain">
    <div class="content">
      <div class="jumbo">
        <img src="../assets/jumbotron.jpg" alt="" />
      </div>
      <!-- Here goes the grid -->
      <div class="sectionTag">
        <div class="tagText">CURRENT SERIES</div>
      </div>
      <div class="row">
        <Card
          v-for="card in cards"
          :key="card.ID"
          :comicImg="card.thumb"
          :comicName="card.series.toUpperCase()"
          class="col_2"
        />
      </div>
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
import Card from "./Card.vue";

export default {
  name: "SiteMain",
  components: {
    Card,
  },
  data() {
    return {
      cards: [
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
@import;
.siteMain {
  position: relative;
  z-index: 1;
  // height: 236px;
  background-color: black;

  .content {
    // height: 118px;

    .jumbo {
      height: 400px;

      img {
        width: 100%;
        height: 100%;
        object-position: top;
        object-fit: cover;
      }
    }

    .sectionTag {
      transform: translate(0, -50%);
      width: 70%;
      margin: auto;
      color: white;

      .tagText {
        font-weight: bold;
        font-size: 1.3rem;
        width: 250px;
        height: 50px;
        background-color: cornflowerblue;
        line-height: 50px;
        text-align: center;
      }
    }

    .row {
      margin: auto;
      width: 70%;
      display: flex;
      flex-wrap: wrap;
      padding: 1rem;
    }

    .col_2 {
      width: calc(100% / 6);
      // height: calc(100% / 2);

      img {
        padding: 1rem;
        height: 185px;
        width: 185px;
        object-fit: cover;
        object-position: top;
      }
    }

    h3 {
      padding: 2px 1rem;
      color: white;
      font-size: 0.8rem;
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
