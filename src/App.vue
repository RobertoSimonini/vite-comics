<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'
export default {
  name: 'comics', 
  components: {AppHeader, AppMain, AppFooter}
}
</script>


<template>

  
    <app-header></app-header>
    <app-main></app-main>
    <app-footer></app-footer>
  

</template>

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  /* Generics  */

  body { font-family: "Open Sans Condensed", sans-serif; }


  .container {
    max-width: 75%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
  }

  ul {
    list-style-type: none;
  }

  a {
    text-decoration: none;
  }

</style>