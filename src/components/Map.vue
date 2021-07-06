<template>
  <GoogleMap
  api-key="AIzaSyCg_pPq-VFcOXMl-t_O_kX4IPxrF0S6zJU"
  style="width: 100%; height: 400px"
  :center="center"
  :zoom="15"
  >
    <Marker :options="{ position: center }" />
  </GoogleMap>
  <h5>Find me</h5>
  <div class="address">{{ address }}</div>
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
    padding-left: 50px;
    margin-top: 30px;
}

.address{
    padding-left: 50px;
}
</style>