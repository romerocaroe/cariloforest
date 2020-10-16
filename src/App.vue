<template>
  <div id="app">
        <guestMain></guestMain>
  </div>
</template>

<script>
import GuestMain from './components/Form/GuestMain';

export default {
  name: "App",
  components: {
    GuestMain
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  font-weight: bold;
}

body {
  background: #ADBCC9;
}
</style>
