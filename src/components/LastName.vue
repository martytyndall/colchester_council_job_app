<template>
    <div class="lastname-container">
        <h5>Last name <span class="danger">*</span></h5>
        <input type="text" required>
    </div>
    
    
</template>

<script>

export default{
    name: 'LastName',

    props: {
    },

    components: {
    },
}
</script>

<style scoped>
    .lastname-container{
        float: right;
        padding-left: 15px;
    }
    
    .lastname-container input{
        width: 270px;
        height: 40px;
    }
    
</style>