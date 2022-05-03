<template>
  <nav>
    <ul>
      <li v-for="(title, index) in navMenu" :key="index">
        <a href="#">{{ title }}</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "NavComponent",
  data() {
    return {
      navMenu: [
        "Characters",
        "Comics",
        "Movies",
        "Tv",
        "Games",
        "Collectables",
        "Videos",
        "Fans",
        "News",
        "Shop",
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/sass/partials/variables";
ul {
  list-style: none;
  display: flex;
  justify-content: center;
  align-content: center;
  li {
    padding: 0 1rem;

    a {
      text-decoration: none;
      text-transform: uppercase;
      font-size: 14px;
      font-weight: 400;
      padding: 3.125rem 0;
      color: black;
    }

    &:nth-child(2) a {
      color: $primaryColor;
      box-shadow: 0px 8px $primaryColor;
    }
  }
}
</style>