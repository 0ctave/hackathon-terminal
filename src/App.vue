<template>
  <div id="app">
    <div class="container">

      <Check v-if="checking"/>
      <Panel v-if="!checking"/>
      <div v-if="!checking" class="wrapper">
        <div class="welcome">
          <p>Bienvenue<br>PRENOM NOM<br>Sur ton espace personnel</p>
        </div>
        <Calendar class="menu"/>

      </div>
      <Weather v-if="!checking"/>

    </div>
  </div>
</template>

<script>
import Check from './components/Check.vue'
import Panel from './components/Panel.vue'
import Calendar from './components/Calendar.vue'
import Weather from './components/Weather.vue'

export default {
  name: 'App',
  components: {
    Check,
    Panel,
    Calendar,
    Weather,
  },
  data() {
    return {
      checking: true,
      timer: ''

    }
  },
  created() {
    this.timer = setInterval(this.fetchEventsList, 3000);
  },
  methods: {
    fetchEventsList() {
      this.checking = false;
    },
    cancelAutoUpdate() {
      clearInterval(this.timer);
    }
  },
  beforeDestroy() {
    this.cancelAutoUpdate();
  }
}
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Lato");


#app {
  height: 100%;
  display: flex;
  background: linear-gradient(45deg, #70298C, #3192EB, #C5C1A1);
  font-family: "HelveticaNeue-Light", "Helvetica Neue Light", "Helvetica Neue", Helvetica, Arial, "Lucida Grande", sans-serif !important;
  font-weight: 400 !important;
}

body {
  margin: 0;
  height: 100vh;
  font-family: "Lato", sans-serif;
  font-weight: bold;
  font-size: 1.5rem;
  text-transform: uppercase;
  padding: 0;
  overflow: hidden;
}

.container {
  width: 60%;
  margin: auto;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.wrapper {
  width: 80%;
}

.menu {
  width: 40%;
  float: right;
}

.welcome {
  width: 50%;
  float: left;
  padding-top: 60px;
  text-align: right;
  color: white;
}

.fit {
  width: 60%;
}

</style>
