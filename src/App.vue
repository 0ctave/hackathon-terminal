<template>
  <div id="app">
    <div class="container">

    <Check/>
    </div>
  </div>
</template>

<script>
import Check from './components/Check.vue'

export default {
  name: 'App',
  components: {
    Check
  }

}
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Lato");


#app {
  height: 100%;
  display: flex;
  background: linear-gradient(45deg, #70298C, #3192EB, #C5C1A1);
}

body {
  margin: 0;
  height: 100vh;
  font-family: "Lato", sans-serif;
  font-weight: bold;
  font-size: 1.5rem;
  text-transform: uppercase;
}

.container {
  margin: auto;
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
