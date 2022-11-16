<script>
export default {
  name: "AppFooter",
};
</script>

<template>
  <footer>
    <div class="container">
      <div class="footer-top">
        <div class="f-top-left">
          <div class="list-wrap-2-in-1">
            <ul>
              <h2>dc comics</h2>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">Tv</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
            <ul>
              <h2>SHOP</h2>
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
          </div>
          <ul>
            <h2>dc</h2>
            <li><a href="#">Terms Of Use</a></li>
            <li><a href="#">Privacy Policy (news)</a></li>
            <li><a href="#">Ad Choices</a></li>
            <li><a href="#">Advertising</a></li>
            <li><a href="#">Jobs</a></li>
            <li><a href="#">Subscriptions</a></li>
            <li><a href="#">Talent Workshops</a></li>
            <li><a href="#">CPSC Certificates</a></li>
            <li><a href="#">Ratings</a></li>
            <li><a href="#">Shop Help</a></li>
            <li><a href="#">Contact Us</a></li>
          </ul>
          <ul>
            <h2>sites</h2>
            <li><a href="#">DC</a></li>
            <li><a href="#">MAD Magazine</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Universe</a></li>
            <li><a href="#">DC Power Visa</a></li>
          </ul>
        </div>
        <div class="f-top-right">
          <!-- <img src="../assets/img/dc-logo-bg.png" alt="" /> -->
        </div>
      </div>
      <div class="footer-bottom"></div>
    </div>
  </footer>
</template>


<style lang="scss" scoped>
.container {
  background-image: url("../assets/img/dc-logo-bg.png");
  background-position: right;
  background-repeat: no-repeat;
  background-size: 50%;
  overflow-y: hidden;
}
footer {
  background-image: url("../assets/img/footer-bg.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  .footer-top {
    display: flex;
    justify-content: space-between;
    .f-top-left {
      display: flex;
      ul {
        padding: 20px;
        list-style: none;
        h2 {
          text-transform: uppercase;
          margin: 15px 0px;
          color: white;
        }
        a {
          font-size: 0.9rem;
          line-height: 25px;
          color: white;
          text-decoration: none;
        }
        a:hover {
          text-decoration: underline;
        }
      }
    }
  }
}
</style>