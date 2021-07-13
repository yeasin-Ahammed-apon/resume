<template>
  <div id="app">
    <div id="nav">
      <navbar/>
      <!-- <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> -->
    </div>
    <router-view/>
  </div>
</template>
<script>
import Navbar from './components/home/Navbar.vue'
export default {
  components: { 
    Navbar,
   },
}
</script>

<style>

</style>
