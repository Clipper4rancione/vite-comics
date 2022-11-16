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

  img {
    object-fit: cover;
  }
  .text-area {
    margin-top: 15px;
  }
  span {
    font-size: 1rem;
  }
}
</style>