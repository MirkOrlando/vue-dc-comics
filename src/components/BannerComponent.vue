<template>
  <div class="banner">
    <div class="container">
      <div class="row pt-4 pb-4">
        <div
          class="col col-5 text-center"
          v-for="(item, index) in items"
          :key="index"
        >
          <div class="wrapper">
            <img :src="item.src" alt="" />
            <div class="text">{{ item.text }}</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BannerComponent",
  data() {
    return {
      items: [
        {
          id: 1,
          src: require("@/assets/img/buy-comics-digital-comics.png"),
          text: "digital comix",
        },
        {
          id: 2,
          src: require("@/assets/img/buy-comics-merchandise.png"),
          text: "dc merchandise",
        },
        {
          id: 3,
          src: require("@/assets/img/buy-comics-subscriptions.png"),
          text: "subscription",
        },
        {
          id: 4,
          src: require("@/assets/img/buy-comics-shop-locator.png"),
          text: "comic shop lacator",
        },
        {
          id: 5,
          src: require("@/assets/img/buy-dc-power-visa.svg"),
          text: "dc power visa",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.banner {
  background-color: $primaryColor;
  color: $lightestColor;

  .wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 0.5rem;
    transition: all 250ms linear;
    cursor: pointer;
    &:hover {
      transform: translate(0, -10px);
    }

    img {
      height: 50px;
    }

    .text {
      text-transform: uppercase;
    }
  }
}
</style>