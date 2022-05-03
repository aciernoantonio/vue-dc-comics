<template>
  <div id="app">

  <SiteHeader/>

  <SiteMain/>    

  </div>
</template>

<script>

import SiteHeader from "@/components/headerComponent.vue"
import SiteMain from "@/components/mainComponent.vue"


export default {
  name: 'headerComponent',
  components: {
    SiteHeader,
    SiteMain
  }
}
</script>

<style lang="scss">

@import "@/assets/scss/style";

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}


</style>
