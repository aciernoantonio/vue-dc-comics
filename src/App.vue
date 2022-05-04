<template>
  <div id="app">

  <SiteHeader/>

  <SiteMain/> 

  <SiteFooter/>   

  </div>
</template>

<script>

import SiteHeader from "@/components/headerComponent.vue"
import SiteMain from "@/components/mainComponent.vue"
import SiteFooter from "@/components/footerComponent.vue"


export default {
  name: 'headerComponent',
  components: {
    SiteHeader,
    SiteMain,
    SiteFooter
  },

  

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
