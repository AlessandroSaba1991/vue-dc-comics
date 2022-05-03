<template>
  <div id="app">
    <SiteHeader />
  </div>
</template>

<script>
import SiteHeader from './components/HeaderComponent.vue'

export default {
  name: 'App',
  components: {
    SiteHeader
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
}

#app{
  font-family: 'Fira Sans Condensed', sans-serif;
}
</style>
