<template>
  <div id="app">
    <page-header></page-header>
    <section-api> </section-api>    
  </div>
</template>

<script>
import PageHeader from './components/PageHeader.vue'
import SectionApi from './components/SectionApi';
export default {
  name: 'App',
  components:{
    PageHeader,
     SectionApi,
  }
}
</script>

