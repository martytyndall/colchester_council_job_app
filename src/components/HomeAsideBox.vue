<template>

<div class="home-aside1">
    <ContactBox />
</div>
<div class="home-aside2">
    <div class="img-box"></div>
</div>
</template>

<script>
// @ is an alias to /src
import ContactBox from '@/components/ContactBox'


export default {
    name: 'HomeAsideBox',
    components: {
      ContactBox,

    },

    data(){
        return{
        };
    },

    
}
</script>

<style scoped>
    .home-aside1{
        background-color: #F2F2F2;
        width: 360px;
        height: 130px;
        float: right;
    }
    
    .home-aside2{        
        float: right;
        margin-top: 50px;
    }
    
    .img-box{
        background-image: url('src/assets/image2.jpg');
        background-repeat: no-repeat; 
        width: 360px;
        height: 222px;       
    }
    
</style>
