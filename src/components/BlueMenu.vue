<script>
export default {
  name: "BlueMenu",
  data() {
    return {
      blueMenu: [
        {
          image: "buy-comics-digital-comics.png",
          text: "DIGITAL COMICS",
        },

        {
          image: "buy-comics-merchandise.png",
          text: "DC MERCHANDISE",
        },

        {
          image: "buy-comics-subscriptions.png",
          text: "SUBSCRIPTIO",
        },

        {
          image: "buy-comics-shop-locator.png",
          text: "COMIC SHOP LOCATOR",
        },

        {
          image: "buy-dc-power-visa.svg",
          text: "DC POWER VISA",
        },
      ],
    };
  },
};
</script>

<template>
  <section class="blue-menu">
    <div class="container">
      <div class="bm-link">
        <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
        <span>DIGITAL COMICS</span>
      </div>
    </div>
  </section>
</template>


<style lang='scss' scoped>
.blue-menu {
  background-color: #3b7ef0;
  padding: 10px;
  .bm-link {
    display: flex;
    align-items: center;
    width: calc(100% / 5);
    img {
      width: 65px;
      vertical-align: middle;
    }
    span {
      margin-left: 15px;
      color: white;
    }
  }
}
</style>