<script>

  
  import AppMain from './components/AppMain.vue';

  import AppHeaderComp from './components/AppHeaderComp.vue';

  import AppFooterComp from './components/AppFooterComp.vue';

  export default {

    data() {
      return {
        
      }
    },

    components: {
      AppHeaderComp, 
      AppMain,
      AppFooterComp

    }


  }

</script>

<template>

  <!-- APP HEADER -->
    <app-header-comp></app-header-comp>

  <!-- APP MAIN -->
    <app-main></app-main>

    <app-footer-comp></app-footer-comp>

</template>

<style lang="scss" as *>

  @use './style/general.scss';

</style>
