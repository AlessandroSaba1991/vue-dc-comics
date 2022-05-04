<template>
  <div class="sub_main_component">
    <div class="container">
      <div class="row">
        <div class="col" v-for="({ name, image,id }) in MainList" :key="id">
          <div class="card">
            <div class="img">
              <img :src="image" :alt="name" />
            </div>
            <div class="text">{{ name }}</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SubMainComponent",
  data() {
    return {
      MainList: [
        {
          id: 1,
          name: "Digital comics",
          image: require('@/assets/img/buy-comics-digital-comics.png'),
        },
        {
          id: 2,
          name: "Dc Merchandise",
          image: require('@/assets/img/buy-comics-merchandise.png'),
        },
        {
          id: 3,
          name: "Subscription",
          image: require('@/assets/img/buy-comics-subscriptions.png'),
        },
        {
          id: 4,
          name: "Comic Shop Locator",
          image: require('@/assets/img/buy-comics-shop-locator.png'),
        },
        {
          id: 5,
          name: "Dc Power visa",
          image: require('@/assets/img/buy-dc-power-visa.svg'),
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>

.sub_main_component {
  padding: 3rem;
  background-color: $primaryColor;
  .card {
    display: flex;
    justify-content: center;
    align-items: center;
    column-gap: 0.5rem;
    .img{
        height: 50px;  
        aspect-ratio: 1 / 1;  
        display: flex;
    }
    .text{
        color: $white;
        text-transform: uppercase;
    }
  }
}
</style>