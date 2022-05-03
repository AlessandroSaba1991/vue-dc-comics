<template>
  <main>
    <SectionContent />
    <SectionMerchandise />
  </main>
</template>

<script>
import SectionContent from './MainSectionContentComponent.vue'
import SectionMerchandise from './MainSectionMerchandiseComponent.vue'
export default {
  name: "MainComponent",
  components:{
      SectionContent,
      SectionMerchandise
  }
};
</script>

