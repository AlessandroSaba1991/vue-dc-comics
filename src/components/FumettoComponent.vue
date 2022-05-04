<template>
  <div class="col_2">
    <div class="card">
      <div class="img">
        <img :src="fumetto.thumb" :alt="fumetto.type" />
      </div>
      <div class="text">
        <small>{{ fumetto.series }}</small>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FumettoComponent",
  props: {
    fumetto: Object,
  },
};
</script>

<style lang="scss" scoped>
.card {
  padding: 1rem;
  .img {
    
    img {
      aspect-ratio: 1 / 1;
      object-fit: cover;
      object-position: top;
    }
  }
  .text {
    color: $white;
    margin-top: 0.5rem;
    text-transform: uppercase;
  }
}
</style>