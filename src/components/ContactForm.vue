<template>

<div class="contact-container">
    <form action="/">
        <div class="contact-input-fields">
            <FirstName />
            <LastName />
        </div>
        <Email />
        <Telephone />
        <DOB />
        <Address />      
        <Message />
        <br>
        <input type="submit" class="btn" id="submit-button" value="Send your message">

    </form>
</div>

      
      
</template>

<script>
// @ is an alias to /src
import FirstName from '@/components/FirstName.vue'
import LastName from '@/components/LastName.vue'
import Email from '@/components/Email.vue'
import Telephone from '@/components/Telephone.vue'
import DOB from '@/components/DOB.vue'
import Address from '@/components/Address.vue'
import Message from '@/components/Message.vue'

export default {
    name: 'ContactForm',
    components: {
        FirstName,
        LastName,
        Email,
        Telephone,
        DOB,
        Address,
        Message,
        },
    methods: {
        
    },
}

var formValidated = false;

</script>

<style scoped>
    .contact-container{
        background-color: #F2F2F2;
        width: 615px;
        height: 1115px;
        float: left;
    }

    .name-container{
        margin-top: 20px;
        height: 30px;
    }

    #submit-button{
        margin-left: 30px;
    }

    @media screen and (max-width: 592px){
        .contact-container{
            width: 100%;
        }

        .aside-container1{
            width: 100%;
            float: none;
        }
        .aside-container2{
            width: 100%;
            float: none;
        }
        
    }
    
</style>
