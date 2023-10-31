 <template >
<!--     <headBlock></headBlock>
    <App></App>
    <footerBlock></footerBlock>
    <headBlock></headBlock>
    <blog></blog>
    <footerBlock></footerBlock>
    <headBlock></headBlock>
    <blogDetails></blogDetails>
    <footerBlock></footerBlock> -->
      <Header></Header>
    <router-view></router-view>
<!--     <Project_details></Project_details> -->
    

    
</template>

<script>


import Header from "./components/Header.vue";
export default {

    components: {
        Header,
    }
  






};
</script>
<style lang="scss">

</style> 
