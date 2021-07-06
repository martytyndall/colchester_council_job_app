<template>
  <div class="aside-container1">
    <Map  />     
  </div>
  <div class="aside-container2">
    <h5>Follow me</h5>   
    <i class="fa fa-facebook" aria-hidden="true"></i>  
    <i class="fa fa-twitter" aria-hidden="true"></i>  
    <i class="fa fa-linkedin" aria-hidden="true"></i>  
    <i class="fa fa-youtube" aria-hidden="true"></i>
  </div>
</template>

<script>
// @ is an alias to /src
import Map from '@/components/Map.vue'
import VueSocial from "@growthbunker/vuesocial"


export default {
  name: 'AsideBox',
  components: {
    Map,
    VueSocial,
    }
}
</script>

<style scoped>
    .aside-container1{
        background-color: #F2F2F2;
        width: 360px;
        height: 600px;
        float: right;
    }
    .aside-container2{
        background-color: #F2F2F2;
        width: 360px;
        height: 200px;
        float: right;
        margin-top: 50px;
        border-top: 6px solid #08454E;
    }

    h5{
      padding-left: 50px;
      margin-top: 30px;
    }

    .aside-container2 i {
      font-size: 50px;
      text-decoration: none;
      padding-left: 60px;
      margin-top: 50px;
      width: 60px;
      height: 60px;
      text-align: center;
    }

    .fa-facebook{
      color: #4360B4;
    }
    
    .fa-twitter{
      color: #41AAF1;
    }
    
    .fa-linkedin{
      color: #0072B1;
    }
    
    .fa-youtube{
      color: #FF0000;
    }
    



    
</style>
