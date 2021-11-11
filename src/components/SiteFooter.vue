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
        <div class="rightCol"></div>
        <div class="logoBig">
          <img src="../assets/dc-logo-bg.png" alt="" />
        </div>
      </div>
    </div>
    <div class="contacts"></div>
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

  .linkBlock {
    height: calc(100vh - 454px);
    background-image: url("../assets/footer-bg.jpg");

    .links {
      width: 70%;
      display: flex;
      justify-content: space-between;
    }

    .logoBig {
      img {
        transform: translate(0, -20%);
        // max-height: calc(100vh - 454px);
        width: 100%;
        object-fit: cover;
      }
    }
  }

  .contacts {
    position: relative;
    height: 100px;
    background-color: gray;
    z-index: 2;
  }
}
</style>
