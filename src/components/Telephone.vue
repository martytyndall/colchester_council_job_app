<template>
    <div class="contact-input-fields">
        <h5>Telephone number<span class="danger"> *</span></h5>
        <input type="tel" placeholder="+44" required>
    </div>
    
    
</template>

<script>

export default{
    name: 'Telephone',

    props: {
    },

    components: {
    },
}
</script>

<style scoped>
   

    input{
        width: 555px;
        height: 40px;
        padding-left: 10px;
    }
    
</style>