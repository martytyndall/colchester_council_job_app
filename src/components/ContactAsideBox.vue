<template>
  <div class="aside-container1">
    <Map />
  </div>
  <div class="aside-container2">
    <Socials />
  </div>
</template>

<script>
// @ is an alias to /src
import Map from '@/components/Map.vue'
import Socials from '@/components/Socials'


export default {
  name: 'ContactAsideBox',
  components: {
    Map,
    Socials,
    },
    
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
        padding-left: 50px;
        padding-top: 30px;

    }

    
    @media screen and (max-width: 592px){

        .aside-container1{
            width: 100%;
            height: 600px;
        }
        .aside-container2{
            width: 100%;
            height: 200px;
        }
        
    }



    
</style>
