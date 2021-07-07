<template>
    <div class="contact-input-fields" id="address-input">
        <h1>Do you live in Colchester?<span class="danger"> *</span></h1>
        <form action="" class="address-form" @change="radioChecked()">
            <input type="radio" name="choice" id="yes" value="yes" checked="checked"><h5>Yes</h5>
            <input type="radio" name="choice" id="no" value="no"><h5>No</h5>
        </form>
        <br><br><br><br>
        <h1>What is your home address?<span class="danger"> *</span></h1>
        <br>
        <form action="" class="postcode-form" id="postcode-form">
            <h5>Postcode <span class="danger"> *</span></h5>
            <input class="postcode-input" type="text" placeholder="CO3 3WG">
            <br><br>
            <button class="btn">Find Address</button>
        </form>
        <form action="" class="address-input" id="address-input">
            <h5>Address line 1 <span class="danger"> *</span></h5>
            <input type="text">
            <h5>Address line 2 <span class="danger"> *</span></h5>
            <input type="text">
            <h5>Town/City <span class="danger"> *</span></h5>
            <input type="text">
            <h5>Country <span class="danger"> *</span></h5>
            <input type="text">
            <h5>Postcode <span class="danger"> *</span></h5>
            <input type="text">
        </form>
    </div>
    
    
</template>

<script>

export default{
    name: 'Address',
    methods: {
        radioChecked(){
            const rbs = document.querySelectorAll('input[name="choice"]');
            let selectedValue;
            for (var rb of rbs) {
                if (rb.checked) {
                    selectedValue = rb.value;
                }

                if(selectedValue == "yes"){
                document.getElementById("postcode-form").classList.add("display");
                document.getElementById("address-input").classList.add("hidden");
            } else {
                document.getElementById("postcode-form").classList.add("hidden");
                document.getElementById("address-input").classList.add("display");
            }
            }
            
            
        }
    }
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

    .hidden{
        display: none;
    }

    .display{
        display: block;
    }
    
</style>