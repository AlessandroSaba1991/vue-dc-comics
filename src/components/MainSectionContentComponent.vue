<template>
    <section class="content">
        <div class="container">
      <div class="row">
        <h2>-- Content goes here --</h2>
      </div>
    </div>
    </section>
</template>

<script>
export default {
    name:'MainSectionContentComponent'
}
</script>

<style lang="scss" scoped>
@import "@/assets/sass/partials/variables";
.content {
  padding: 2rem;
  background-color: $bgMain;
  color: white;
}
</style>