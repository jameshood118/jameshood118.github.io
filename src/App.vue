<template>
  <div id="app">
    <div class="columns">
      <div class="column">
        <nav-bar />
      </div>
    </div>
    <div class="container is-fluid">
      <div class="columns">
        <div class="column">
          <router-view/>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
import Bulma from "bulma"
import NavBar from "./components/Navbar.vue"

export default {
  name: 'App',
  components: {
    NavBar
  },
}
</script>

<style>
</style>
