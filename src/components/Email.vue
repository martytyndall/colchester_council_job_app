<template>
    <div class="contact-input-fields">
        <h5>Email address<span class="danger"> *</span></h5>
        <input type="email" placeholder="e.g joe.bloggs@gmail.com" required>
    </div>
    
    
</template>

<script>

export default{
    name: 'Email',

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