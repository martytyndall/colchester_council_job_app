<template>
  <div class="contact-page container">
    <Header title="Marty Tyndall" heading="Send me a message" />
    <ContactForm />
    <ContactAsideBox />


  </div>

</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import ContactForm from '@/components/ContactForm.vue'
import ContactAsideBox from '@/components/ContactAsideBox.vue'

export default {
  name: 'Contact',
  components: {
    Header,
    ContactForm,
    ContactAsideBox,
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
