<template>
  <div id="app">
    <page-header></page-header>
    <section-api> </section-api>    
     <Footer></Footer>
  </div>
</template>

<script>
import PageHeader from './components/PageHeader.vue'
import SectionApi from './components/SectionApi';
import Footer from './components/Footer.vue';
export default {
  name: 'App',
  components:{
    PageHeader,
     SectionApi,
     Footer
  }
}
</script>

