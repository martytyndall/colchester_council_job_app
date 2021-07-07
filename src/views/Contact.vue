<template>
  <div class="contact-page container">
    <Header title="Marty Tyndall" heading="Send me a message" />
    <ContactForm />
    <AsideBox />


  </div>

</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import ContactForm from '@/components/ContactForm.vue'
import AsideBox from '@/components/AsideBox.vue'

export default {
  name: 'Contact',
  components: {
    Header,
    ContactForm,
    AsideBox,
    },

}
</script>

<style scoped>

@media screen and (max-width: 592px) {
  .container{
    height: 2500px;
  }  
}
    
</style>
