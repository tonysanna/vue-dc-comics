<template>
  <div id="app">
    <Header/>
    <Jumbo/>
    <Main/>
    <Footer/>
    
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Main from './components/Main.vue'
import Footer from './components/Footer.vue'
import Jumbo from './components/Jumbo.vue'




export default {
  name: 'App',
  components: {
    Header ,
    Jumbo,
    Main,
    Footer,
    
  }
}
</script>

<style lang="scss">
  @import "./style/comun";
  @import "./style/mixing";
  @import "./style/mood";

</style>
