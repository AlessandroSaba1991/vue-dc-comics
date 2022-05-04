<template>
  <div class="col">
    <div class="card">
      <div class="img">
        <img :src="title.image" :alt="title.name" />
      </div>
      <div class="text">{{ title.name }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MerchandiseComponent",
  props: {
    title: Object,
  },
};
</script>

<style lang="scss" scoped>
.card {
  display: flex;
  justify-content: center;
  align-items: center;
  column-gap: 0.5rem;
  .img {
    height: 50px;
    aspect-ratio: 1 / 1;
    display: flex;
  }
  .text {
    color: $white;
    text-transform: uppercase;
  }
}
</style>