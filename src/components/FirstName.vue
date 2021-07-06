<template>
    <div class="firstname-container">
        <h5>First name <span class="danger">*</span></h5>
        <input type="text">
    </div>
    
    
</template>

<script>

export default{
    name: 'FirstName',

    props: {
    },

    components: {
    },
}
</script>

<style scoped>
    .firstname-container{
        float: left;
        /* padding-left: 10px; */
        
    }
   
    .firstname-container input{
        width: 270px;
        height: 40px;
    }
    
</style>