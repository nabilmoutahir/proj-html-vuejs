<script>

    import AppMainAbout from './AppMainAbout.vue';

    import AppMainWhy from './AppMainWhy.vue';

    import AppMainRecent from './AppMainRecent.vue';

    import AppMainQuote from './AppMainQuote.vue';

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
        }
    }


</script>

<template>

    <AppMainAbout/>

    <AppMainWhy/>

    <AppMainRecent/>

    <AppMainQuote/>

</template>

<style lang="scss" scoped>

</style>