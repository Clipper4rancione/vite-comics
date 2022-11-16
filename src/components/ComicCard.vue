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
      <i class="bi bi-cart-plus"></i>

      <img :src="comic.thumb" :alt="comic.series" />
    </div>

    <div class="text-area">
      <span>{{ comic.series }}</span>
      <p>{{ comic.price }}</p>
    </div>
  </div>
</template>


<style lang="scss" scoped>
.card-cont {
  width: calc(100% / 6);
  height: calc(100% / 2);
  padding: 20px;
  .img-area {
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
    position: relative;
  }

  i {
    display: none;
    position: absolute;
    font-size: 3rem;
  }
  .img-area:hover i {
    display: block;
  }

  .img-area:hover {
    filter: brightness(0.5);
  }
  img {
    object-fit: cover;
  }
  .text-area {
    display: flex;
    flex-direction: column;
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