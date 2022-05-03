<template>
  <div class="sub_main_component">
    <div class="container">
      <div class="row">
        <div class="col" v-for="({ name }, index) in MainList" :key="index">
          <div class="card">
            <div class="img">
              <img src="@/assets/img/buy-comics-merchandise.png" :alt="name" />
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
          name: "Digital comics",
          image: "src/assets/img/buy-comics-digital-comics.png",
        },
        {
          name: "Dc Merchandise",
          image: "./assets/img/buy-comics-merchandise.png",
        },
        {
          name: "Subscription",
          image: "./assets/img/buy-comics-subscriptions.png",
        },
        {
          name: "Comic Shop Locator",
          image: "./assets/img/buy-comics-shop-locator.png",
        },
        {
          name: "Dc Power visa",
          image: "./assets/img/buy-dc-power-visa.svg",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/assets/sass/partials/variables";
.sub_main_component {
  padding: 3rem;
  background-color: $primaryColor;
  .card {
    display: flex;
    justify-content: center;
    align-items: center;
    column-gap: 0.5rem;
    .img{
        width: 50px;
    }
    .text{
        color: white;
        text-transform: uppercase;
    }
  }
}
</style>