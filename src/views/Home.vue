<template>
  <div class="home container">
    <Header title="Marty Tyndall" heading="I am applying for the role of Web 
        Developer at Colchester Borough Council." />
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue'

export default {
  name: 'Home',
  components: {
    Header,
  }
}
</script>
