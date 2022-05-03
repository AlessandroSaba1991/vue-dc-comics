<template>
  <header>
    <div class="container">
      <div class="row align_center">
        <div class="col_1">
          <img src="@/assets/img/dc-logo.png" alt="" />
        </div>
        <div class="col_7 ms-auto">
          <nav>
            <ul>
              <li v-for="(title, index) in navMenu" :key="index">
                <a href="#">{{ title }}</a>
              </li>
            </ul>
          </nav>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderComponent",
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
header {
  padding: 1rem;
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
        padding: 2rem 0;
        color: black;
      }

      &:nth-child(2) a {
        color: $primaryColor;
        box-shadow: 0px 8px $primaryColor;
      }
    }
  }
}
</style>