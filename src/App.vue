<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
export default {
  name: 'comics', 
  components: {AppHeader, AppMain}
}
</script>


<template>

  <div class="container">
    <app-header></app-header>
    <app-main></app-main>
  </div>

</template>

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  /* Generics  */

  ul {
    list-style-type: none;
  }

  a {
    color: black;
    text-decoration: none;
    text-transform: uppercase;
  }

</style>