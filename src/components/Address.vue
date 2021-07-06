<template>
    <div class="contact-input-fields" id="address-input">
        <h1>Do you live in Colchester?<span class="danger">*</span></h1>
        <form action="" class="address-form">
            <input type="radio"><h5>Yes</h5>
            <input type="radio"><h5>No</h5>
        </form>
        <br><br><br><br>
        <h1>What is your home address?<span class="danger">*</span></h1>
        <br>
        <form action="" class="postcode-form">
            <h5>Postcode <span class="danger">*</span></h5>
            <input class="postcode-input" type="text" placeholder="CO3 3WG">
            <br><br>
            <button class="btn">Find Address</button>
        </form>
    </div>
    
    
</template>

<script>

export default{
    name: 'Address',

    props: {
    },

    components: {
    },
}
</script>

<style scoped>

    #address-input{
        height: auto;
    }
        
    .address-form *{
        width: 40px;
        height: 40px;
        float: left;        
    }

    .address-form{
        margin-top: 20px;
        width: 100%;
    }

    .address-form h5{
        transform: translateY(25%);
        margin-left: 10px;
    }

    .address-form input{
        margin-left: 10px;
    }

    .postcode-input{
        width: 360px;
        height: 40px;
    }
    
</style>