<template>
  <div class="sub_main_component">
    <div class="container">
      <div class="row">
        <MerchandiseItem :title="title" v-for="title in MainList" :key="title.id"/>
      </div>
    </div>
  </div>
</template>

<script>
import MerchandiseItem from "./MerchandiseComponent.vue";

export default {
  name: "SubMainComponent",
  components: {
    MerchandiseItem,
  },
  data() {
    return {
      MainList: [
        {
          id: 1,
          name: "Digital comics",
          image: require("@/assets/img/buy-comics-digital-comics.png"),
        },
        {
          id: 2,
          name: "Dc Merchandise",
          image: require("@/assets/img/buy-comics-merchandise.png"),
        },
        {
          id: 3,
          name: "Subscription",
          image: require("@/assets/img/buy-comics-subscriptions.png"),
        },
        {
          id: 4,
          name: "Comic Shop Locator",
          image: require("@/assets/img/buy-comics-shop-locator.png"),
        },
        {
          id: 5,
          name: "Dc Power visa",
          image: require("@/assets/img/buy-dc-power-visa.svg"),
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
}
</style>