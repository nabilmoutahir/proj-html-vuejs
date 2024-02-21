<script>

  
  import AppMain from './components/AppMain.vue';

  import AppComps from './components/AppComps.vue';


  export default {

    data() {
      return {
        
      }
    },

    components: {
      AppComps, 
      AppMain

    }


  }

</script>

<template>

  <!-- APP HEADER -->
    <app-comps></app-comps>

  <!-- APP MAIN -->
    <app-main></app-main>

</template>

<style lang="scss" as *>

  @use './style/general.scss';

</style>
