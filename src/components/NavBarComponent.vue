<template>
  <nav>
    <a
      :href="item.href"
      v-for="(item, index) in NavItems"
      :key="index"
      :class="{ active: activeItem === index }"
      @click="activeItem = index"
      >{{ item.text }}</a
    >
  </nav>
</template>

<script>
export default {
  name: "NavBarComponent",
  data() {
    return {
      NavItems: [
        {
          id: 1,
          href: "#",
          text: "characters",
        },
        {
          id: 1,
          href: "#",
          text: "comics",
        },
        {
          id: 1,
          href: "#",
          text: "movies",
        },
        {
          id: 1,
          href: "#",
          text: "tv",
        },
        {
          id: 1,
          href: "#",
          text: "games",
        },
        {
          id: 1,
          href: "#",
          text: "collectibles",
        },
        {
          id: 1,
          href: "#",
          text: "videos",
        },
        {
          id: 1,
          href: "#",
          text: "fans",
        },
        {
          id: 1,
          href: "#",
          text: "news",
        },
        {
          id: 1,
          href: "#",
          text: "shop",
        },
      ],
      activeItem: 1,
    };
  },
};
</script>

<style lang="scss" scoped>
nav {
  display: flex;
  align-items: center;
  height: 100%;

  a {
    color: $darkColor;
    display: flex;
    align-items: center;
    text-transform: uppercase;
    padding: 4rem 1rem;
    margin: 0 0.5rem;
    height: 100%;
    border-bottom: 6px solid transparent;
    font-weight: bold;
    cursor: pointer;
    transition: all 250ms linear;
    &:last-child {
      margin-right: 0;
    }
    &.active {
      color: $primaryColor;
      border-color: $primaryColor;
    }
    &:hover {
      color: $primaryColor;
      border-color: $primaryColor;
    }
  }
}
</style>