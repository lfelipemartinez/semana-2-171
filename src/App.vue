<template>
  <div id="app">
    <page-header></page-header>
    <page-banner></page-banner>
    <section-api> </section-api>    
     <Footer></Footer>
  </div>
</template>

<script>
import PageHeader from './components/PageHeader.vue'
import SectionApi from './components/SectionApi';
import Footer from './components/Footer.vue';
import PageBanner from "./components/PageBanner.vue";
export default {
  name: 'App',
  components:{
    PageHeader,
     SectionApi,
     Footer,
     PageBanner
  }
}
</script>

