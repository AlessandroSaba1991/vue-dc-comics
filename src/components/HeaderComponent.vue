<template>
  <header>
    <div class="container">
      <div class="row align_center">
        <div class="col_1 flex align-center">
          <img width="80" src="@/assets/img/dc-logo.png" alt="logo DC" />
        </div>
        <div class="col_7 ms-auto">
          <NavMenu />
        </div>
      </div>
    </div>
  </header>
</template>

<script>
import NavMenu from "./NavComponent.vue";

export default {
  name: "HeaderComponent",
  components: {
    NavMenu,
  },
};
</script>

<style lang="scss" scoped>
header {
  padding: 1rem;
}
</style>