<script>
import ComicCard from "./ComicCard.vue";
import comic from "../data/dc-comics";

export default {
  name: "AppMain",
  components: {
    ComicCard,
  },
  data() {
    return {
      comic,
    };
  },
};
</script>

<template>
  <main>
    <div class="container">
      <div class="card-wrapper">
        <ComicCard v-for="(item, index) in comic" :key="index" :comic="item" />
      </div>
      <div class="cta">
        <div class="button-show-more">show more</div>
      </div>
    </div>
  </main>
</template>


<style lang="scss" scoped>
main {
  width: 100%;
  color: white;
  background-color: #212121;
  padding: 30px 0px;
  .card-wrapper {
    margin-top: 20px;

    display: flex;
    flex-wrap: wrap;
  }
  .cta {
    text-align: center;
    cursor: pointer;
  }
  .button-show-more {
    text-transform: uppercase;
    padding: 5px 30px;
    display: inline-block;
    background-color: #3b7ef0;
  }
}
</style>