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
          text: "SUBSCRIPTION",
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
  methods: {
    getPathImage(imageName) {
      return new URL(`../assets/img/${imageName}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <section class="blue-menu">
    <div class="container blue-container">
      <div class="bm-link" v-for="(el, index) in blueMenu" :key="index">
        <img :src="getPathImage(el.image)" alt="" />
        <span>{{ el.text }}</span>
      </div>
    </div>
  </section>
</template>



<style lang='scss' scoped>
.blue-menu {
  .blue-container {
    padding: 40px;
    display: flex;
  }
  background-color: #3b7ef0;
  padding: 10px;
  .bm-link {
    display: flex;
    align-items: center;
    width: calc(100% / 5);
    img {
      width: 60px;
      vertical-align: middle;
    }
    span {
      margin-left: 15px;
      color: white;
    }
  }
}
</style>