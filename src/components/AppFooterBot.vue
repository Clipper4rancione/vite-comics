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
        <div class="social section">
          <span>follow us</span>
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
    justify-content: space-between;

    .sign-up-btn {
      font-size: 1.4rem;
      border: 2px solid #3b7ef0;
      padding: 10px 25px;
    }
  }
}
</style>