<template>
    <div class="contact-input-fields" >


        <h1>Do you live in Colchester?<span class="danger"> *</span></h1>
        <div class="radios" >
            <input type="radio" name="choice" id="yes" value="yes" checked="checked" @change="radioChecked(0)"><h5>Yes</h5>
            <input type="radio" name="choice" id="no" value="no" @change="radioChecked(1)"><h5>No</h5>
        </div>


        <br><br><br><br>        
        <h1>What is your home address?<span class="danger"> *</span></h1>
        <br>


        <div class="postcode-form" id="postcode-form">
            <h5>Postcode <span class="danger"> *</span></h5>
            <form @submit.prevent="postcodeData" method="post">
                <input class="postcode-input" type="text" placeholder="CO3 3WG" name="input" v-model="postcode.input" required>
                <br><br>
                <button type="submit" class="btn">Find Address</button>
            </form>            
        </div>

        <div class="hidden" id="your-address">
            <h5>Please select your address from the drop down list <span class="danger"> *</span> </h5>
            <select name="" id="address-list"/>
        </div>
        


        <div class="address-form hidden" id="address-form">
            <h5>Address line 1 <span class="danger"> *</span></h5>
            <input type="text" required>
            <h5>Address line 2</h5>
            <input type="text">
            <h5>Town/City <span class="danger"> *</span></h5>
            <input type="text" required>
            <h5>Country <span class="danger"> *</span></h5>
            <input type="text" required>
            <h5>Postcode <span class="danger"> *</span></h5>
            <input type="text" required>
        </div>
    </div>



</template>

<script>
import axios from 'axios'
import { bus } from '@/main'



export default{
    name: 'Address',
    components: {
    },

    data(){
        return{
            postcode:{
                input:null,
            },
            
        }
    },
    methods: {
        radioChecked(x){
            if(x==0){
                document.getElementById("postcode-form").classList.remove("hidden");
                document.getElementById("address-form").classList.add("hidden");                
            } else {
                document.getElementById("postcode-form").classList.add("hidden");
                document.getElementById("address-form").classList.remove("hidden");     
            }            
        },

        postcodeData(e){
            e.preventDefault();

            const postCode = this.postcode.input;
            const postCodeLength = postCode.length;
            const indexToSplit = postCodeLength - 3;

            let postCodeStart = postCode.substring(0, indexToSplit);
            let postCodeEnd = postCode.substring(indexToSplit);
            postCodeStart = postCodeStart.trim();
            postCodeEnd = postCodeEnd.trim();

            const formattedPostCode = postCodeStart + " " + postCodeEnd;


            axios.get("https://interviewtask.azurewebsites.net/api/address?postcode=" + formattedPostCode)
            .then((response) => {                       
            })
            .catch(function (error) {
                // handle error
                console.log(error);
            })

            document.getElementById("postcode-form").classList.add("hidden");
            document.getElementById("your-address").classList.remove("hidden");
        },

        


       
    },

}





</script>

<style scoped>

    #address-input{
        height: auto;
    }
        
    .radios *{
        width: 40px;
        height: 40px;
        float: left;        
    }

    .radios{
        margin-top: 20px;
        width: 100%;
    }

    .postcode-form{
        height: auto;
        float: left;
        width: 100%;
    }

    .address-form{
        width: 100%;
        height: auto;
        /* margin-top: 20px; */
    }

    .radios h5{
        margin-bottom: 5px;
        transform: translateY(25%);
        margin-left: 5px;
        margin-right: 5px;
        float: left;
    }

    .address-form input{
        width: 555px;
        height: 40px;
    }

    .address-form h5{
        margin-top: 10px;
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