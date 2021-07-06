<template>
  <div class="contact-page container">
    <Header title="Marty Tyndall" heading="Send me a message" />
    <ContactBox />
    <AsideBox />


  </div>

</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'
import ContactBox from '@/components/ContactBox.vue'
import AsideBox from '@/components/AsideBox.vue'

export default {
  name: 'Contact',
  components: {
    Header,
    ContactBox,
    AsideBox,
    }
}
</script>

<style scoped>
    
</style>
