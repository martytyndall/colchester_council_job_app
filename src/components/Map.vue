<template>
  <GoogleMap
  api-key="AIzaSyCg_pPq-VFcOXMl-t_O_kX4IPxrF0S6zJU"
  style="width: 100%; height: 400px"
  :center="center"
  :zoom="15"
  >
    <Marker :options="{ position: center }" />
  </GoogleMap>
  <div class="findMe-container">
      <h5>Find me</h5>
      <div class="address">{{ address }}</div>
  </div>
  
</template>

<script>
import { defineComponent } from 'vue'
import { GoogleMap, Marker } from 'vue3-google-map'

export default defineComponent({
  components: { GoogleMap, Marker },
  setup() {
    const center = { lat: 51.912482, lng: 0.91563 }

    return { center }
  },

  props: {
      
  }
})
</script>

<style scoped>
h5 {
    padding-left: 10px;
    margin-top: 30px;
}

.address{
    padding-left: 10px;
}

.findMe-container{
    height: 80px;
    border-left: 5px solid grey;
    margin-left: 50px;
}
</style>