<template>
    <div class="contact-input-fields">
        <h5>Your message <span class="danger">*</span></h5>
        <form action="">
            <input type="text">
            <br><br>
            <button class="btn">Send your message</button>
        </form>
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
    
</style>