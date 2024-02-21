<script>

    import AppMainAbout from './AppMainAbout.vue';

    import AppMainWhy from './AppMainWhy.vue';

    import AppMainRecent from './AppMainRecent.vue';

    import AppMainQuote from './AppMainQuote.vue';

    import AppMainAdvice from './AppMainAdvice.vue';

    import AppMainForm from './AppMainForm.vue';

    export default {
        data (){
            return {

            }
        },

        components:{
            AppMainAbout, 
            AppMainWhy,
            AppMainRecent,
            AppMainQuote,
            AppMainAdvice,
            AppMainForm
        }
    }


</script>

<template>

    <AppMainAbout/>

    <AppMainWhy/>

    <AppMainRecent/>

    <AppMainQuote/>

    <AppMainAdvice/>
    
    <AppMainForm/>

</template>

<style lang="scss" scoped>

</style>