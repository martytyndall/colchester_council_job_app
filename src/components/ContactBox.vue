<template>
  <div class="contact-container">
      <div class="contact-input-fields">
          <FirstName />
          <LastName />
      </div>
      <!-- <br><br><br><br><br> -->
      <Email />
      <!-- <br><br><br><br><br> -->
      <Telephone />
      <!-- <br><br><br><br><br> -->
      <DOB />
      <!-- <br><br><br><br><br> -->
      <Address />
      <!-- <br><br><br><br><br><br><br><br><br><br> -->
      <!-- <br><br><br><br><br><br><br><br><br><br> -->
      <Message />
      



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
  name: 'ContactBox',
  components: {
      FirstName,
      LastName,
      Email,
      Telephone,
      DOB,
      Address,
      Message,
    }
}
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
    
</style>
