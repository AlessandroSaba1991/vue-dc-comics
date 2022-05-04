<template>
  <div class="top">
    <div class="container">
      <div class="row">
        <div class="col_4 py-3">
          <div class="row">
            <div class="col_4">
              <h3>DC COMICS</h3>
              <ul>
                <li><small>Characters</small></li>
                <li><small>Comics</small></li>
                <li><small>Movies</small></li>
                <li><small>TV</small></li>
                <li><small>Games</small></li>
                <li><small>Videos</small></li>
                <li><small>News</small></li>
              </ul>
              <h3>Shop</h3>
              <ul>
                <li><small>Shop DC</small></li>
                <li><small>Shop DC Collectibles</small></li>
              </ul>
            </div>
            <div class="col_4">
              <h3>DC</h3>
              <ul>
                <li><small>Terms of Use</small></li>
                <li><small>Privacy policy (New)</small></li>
                <li><small>Ad Choise</small></li>
                <li><small>Advertising</small></li>
                <li><small>Jobs</small></li>
                <li><small>Subscriptions</small></li>
                <li><small>Talent Workshop</small></li>
                <li><small>CPSC Certificates</small></li>
                <li><small>Ratings</small></li>
                <li><small>Show Help</small></li>
                <li><small>Contact Us</small></li>
              </ul>
            </div>
            <div class="col_4">
              <h3>SITES</h3>
              <ul>
                <li><small>DC</small></li>
                <li><small>MAD Magazine</small></li>
                <li><small>DC Kids</small></li>
                <li><small>DC Universe</small></li>
                <li><small>DC Power Visa</small></li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col_6 ms-auto">
          <div class="row h_100">
            <div class="col_11 bg"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FooterTopComponent",
};
</script>

<style lang="scss" scoped>
.top {
  background-image: url("@/assets/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  h3 {
    margin-bottom: 1rem;
    color: $white;
  }
  ul {
    list-style: none;
    margin-bottom: 1rem;
    li {
      color: $textFooter;
      line-height: 1.25rem;
    }
  }
}
.bg {
  background-image: url("@/assets/img/dc-logo-bg.png");
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
  margin-left: auto;
  height: 100%;
}

.py-3 {
  padding: 2.5rem 0;
}
</style>