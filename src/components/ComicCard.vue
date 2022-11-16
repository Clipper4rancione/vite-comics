<script>
export default {
  name: "ComicCard",
  props: {
    comic: Object,
  },
};
</script>

<template>
  <div class="card-cont">
    <div class="img-area">
      <div class="hover"></div>
      <img :src="comic.thumb" :alt="comic.series" />
    </div>

    <div class="text-area">
      <span>{{ comic.series }}</span>
    </div>
  </div>
</template>


<style lang="scss" scoped>
.card-cont {
  width: calc(100% / 6);
  height: calc(100% / 2);
  padding: 20px;
  .img-area {
    cursor: pointer;
  }
  .img-area:hover {
    filter: brightness(0.5);
  }
  img {
    object-fit: cover;
  }
  .text-area {
    margin-top: 15px;
  }
  span {
    cursor: pointer;
    font-size: 1rem;
  }
  span:hover {
    text-decoration: underline;
  }
}
</style>