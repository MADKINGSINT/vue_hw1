 <template >
    <headBlock></headBlock>
    <App></App>
    <footerBlock></footerBlock>
    <headBlock></headBlock>
    <blog></blog>
    <footerBlock></footerBlock>
    <headBlock></headBlock>
    <blogDetails></blogDetails>
    <footerBlock></footerBlock>
    

    
</template>

<script>

import blog from "./components/Blog.vue";
import App from "./components/Home.vue";
import blogDetails from './components/Blog_details.vue';
import headBlock from '@/components/Header.vue'
import footerBlock from './components/Footer.vue';

export default {


  components: {
    blog,
    App,
    blogDetails,
    headBlock,
    footerBlock,



  },
  data() {
    return {
      page: 0,

    }
  },
  methods: {
    getPage(page) {
      this.page = page;
    }


  },
  props: {
    page: Number,
  }
};
</script>
<style lang="scss">

</style> 
<!-- 
<script>
import HeaderComponent from "./components/Header.vue";
import blog from "./components/Blog.vue";
import App from "./components/App.vue";
import blogDetails from "./components/Blog_details.vue";

export default {
  components: {
    blog,
    App,
    blogDetails,
    HeaderComponent,
  },
    methods: {
    обработатьЗначение(значение) {
       return значение
      },
      getValue() {
        return this.обработатьЗначение
    }
  },
  data() {
    return {
       currentPage: this.обработатьЗначение()
        
    };
  },

};
</script>

// Главный компонент

<template>
  <div>
    <header-component
      @передача-значения="обработатьЗначение"
    ></header-component>
    остальной код 
  </div>
  <h1>{{ this.currentPage }}</h1>
  <div v-if="обработатьЗначение === 0">
    
  </div>
  <div v-if="getValue=== 1">
    <blog></blog>
  </div>
  <div v-if="getValue === 2">
    <blogDetails></blogDetails>
  </div>
</template>
 -->