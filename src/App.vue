<template>
  <div id="app">
    <SiteHeader />
    <SiteMain />
    <SiteFooter />
  </div>
</template>

<script>
import SiteHeader from './components/HeaderComponent.vue'
import SiteMain from './components/MainComponent.vue'
import SiteFooter from './components/FooterComponent.vue'


export default {
  name: 'App',
  components: {
    SiteHeader,
    SiteMain,
    SiteFooter
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Fira+Sans+Condensed:wght@300;400;500;700&display=swap');
@import '@/assets/sass/style';

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

img{
  max-width: 100%;
  max-height: 100%;
}

#app{
  font-family: 'Fira Sans Condensed', sans-serif;
}
</style>
