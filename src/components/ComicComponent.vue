<template>
  <div class="comic-card">
    <div class="comic-cover">
      <img :src="comic.thumb" :alt="comic.series" />
    </div>
    <div class="comic-title">{{ comic.series }}</div>
  </div>
</template>

<script>
export default {
  name: "ComicsComponent",
  props: {
    comic: Object,
  },
};
</script>

<style lang="scss" scoped>
.comic-card {
  width: calc((100% / 6) - 0.5rem);
  padding: 1rem 0.5rem;
  transition: all 250ms linear;
  &:hover {
    cursor: pointer;
    transform: scale(1.05);
  }
  .comic-cover {
    img {
      width: 100%;
      aspect-ratio: 1 / 1;
      object-fit: cover;
      object-position: top;
    }
  }
  .comic-title {
    padding-top: 0.5rem;
  }
}
</style>