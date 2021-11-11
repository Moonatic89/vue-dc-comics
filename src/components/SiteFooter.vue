<template>
  <div class="siteFooter">
    <div class="linkBlock">
      <div class="links">
        <div class="leftCol">
          <dl>
            <dt>DC COMICS</dt>
            <dd>Characters</dd>
            <dd>Comics</dd>
            <dd>Movies</dd>
            <dd>TV</dd>
            <dd>Games</dd>
            <dd>Videos</dd>
            <dd>News</dd>
          </dl>

          <dl>
            <dt>SHOP</dt>
            <dd>Shop DC</dd>
            <dd>Shop DC Collectibles</dd>
          </dl>
        </div>

        <div class="midCol">
          <dl>
            <dt>DC</dt>
            <dd>Terms of Use</dd>
            <dd>Privacy Policy (New)</dd>
            <dd>Ad Choices</dd>
            <dd>Advertising</dd>
            <dd>Jobs</dd>
            <dd>Subscriptions</dd>
            <dd>Talent Workshop</dd>
            <dd>CPSC Certificates</dd>
            <dd>Ratings</dd>
            <dd>Shop Help</dd>
            <dd>Contact Us</dd>
          </dl>
        </div>

        <div class="rightCol">
          <dl>
            <dt>SITES</dt>
            <dd>DC</dd>
            <dd>MAD Magazine</dd>
            <dd>DC Kids</dd>
            <dd>DC Universe</dd>
            <dd>DC Power Visa</dd>
          </dl>
        </div>
      </div>
      <div class="logoBig">
        <img src="../assets/dc-logo-bg.png" alt="" />
      </div>
    </div>
    <div class="contacts">
      <div class="btn">
        <span> SIGN-UP NOW! </span>
      </div>
      <ul>
        <il>FOLLOW US</il>
        <il>
          <img src="../assets/footer-facebook.png" alt="" />
        </il>
        <il>
          <img src="../assets/footer-twitter.png" alt="" />
        </il>
        <il>
          <img src="../assets/footer-youtube.png" alt="" />
        </il>
        <il>
          <img src="../assets/footer-pinterest.png" alt="" />
        </il>
        <il>
          <img src="../assets/footer-periscope.png" alt="" />
        </il>
      </ul>
    </div>
  </div>
</template>

<script>
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
.siteFooter {
  width: 100%;
  height: calc(100vh - 354px);
  background-color: black;
  background-image: url("../assets/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;

  .linkBlock {
    display: flex;
    justify-content: space-between;
    margin: auto;
    width: 70%;
    height: calc(100vh - 454px);
    align-items: center;

    .links {
      width: 70%;
      display: flex;

      dl {
        color: gray;
        padding: 1rem;
      }

      dt {
        color: white;
        padding: 0.5rem 0;
        font-size: 1.5rem;
      }
    }

    .logoBig {
      img {
        width: 100%;
        object-fit: cover;
      }
    }
  }

  .contacts {
    position: relative;
    height: 100px;
    background-color: rgb(54, 54, 54);
    z-index: 2;
    display: flex;
    justify-content: space-between;
    align-items: center;

    ul:first-child {
      color: chartreuse;
    }
  }
}
</style>
