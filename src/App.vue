<template>

  <div class="mb-5">
    <NavBarVue />
  </div>



<router-view>
    
</router-view>  

  <div class="mt-5">
    <FooterVue />
  </div>


</template>

<script>
import { RouterLink, RouterView } from 'vue-router'

import FooterVue from './views/layout/Footer.vue'
import NavBarVue from './views/layout/NavBar.vue'
import SearchVue from './views/search/Search.vue'
import SearchResult from './views/searchResult/SearchResult.vue';
export default {
  name: 'App',
  components: {
    NavBarVue,
    FooterVue,
    SearchVue,
    SearchResult


  }
}
</script>

<style>
.mb-5{
  margin-bottom: 5%;
}

.mt-5{
  margin-top: 5%;
}
.SearchBox{
  background-image: url('https://assets.brandinside.asia/uploads/2021/01/shutterstock_1456717751-scaled.jpg');
}
</style>