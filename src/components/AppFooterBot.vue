<script>
export default {
  name: "AppFooterBot",
};
</script>

<template>
  <section class="bot-footer">
    <div class="container">
      <div class="wrapper">
        <div class="sign-up-btn">sign-up now!</div>
        <div class="social-section">
          <span>follow us</span>
          <img src="../assets/img/footer-facebook.png" alt="" />
          <img src="../assets/img/footer-twitter.png" alt="" />
          <img src="../assets/img/footer-youtube.png" alt="" />
          <img src="../assets/img/footer-pinterest.png" alt="" />
          <img src="../assets/img/footer-periscope.png" alt="" />
        </div>
      </div>
    </div>
  </section>
</template>


<style lang="scss" scoped>
.bot-footer {
  padding: 15px;
  background-color: #333333;
  .wrapper {
    color: white;
    text-transform: uppercase;
    display: flex;
    align-items: center;
    justify-content: space-between;

    .sign-up-btn {
      cursor: pointer;
      font-size: 1.4rem;
      border: 2px solid #3b7ef0;
      padding: 10px 25px;
    }
    .social-section {
      display: flex;
      align-items: center;
      span {
        font-size: 1.5rem;
        color: #3b7ef0;
      }
      img {
        vertical-align: middle;
        margin-left: 15px;
      }
    }
  }
}
</style>