<template>
    <div class="contact-input-fields" id="message-box">
        <h5>Your message <span class="danger">*</span></h5>
        <input type="text">     
    </div>
    
    
</template>

<script>

export default{
    name: 'Message',

    props: {
    },

    components: {
    },
}
</script>

<style scoped>
    
    input{
        width: 555px;
        height: 200px;
        padding-left: 10px;
    }

    #message-box{
        height: auto;
    }
    
</style>