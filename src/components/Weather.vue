<template>
<div>
  <vue-weather
      api-key="1dc51bdb19405ce157a316a9efa10afe"
      units="fr"
      latitude="24.8864"
      longitude="91.8807"
      bar-color="white"
      text-color="white"
  />
</div>
</template>

<script>
import VueWeather from "vue-weather-widget";

export default {
  name: "Weather",
  components: {
    VueWeather,
  },
}
</script>

<style scoped>

</style>