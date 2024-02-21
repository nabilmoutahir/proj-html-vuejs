<script>

    import AppMainAbout from './AppMainAbout.vue';

    import AppMainWhy from './AppMainWhy.vue';

    import AppMainRecent from './AppMainRecent.vue';

    export default {
        data (){
            return {

            }
        },

        components:{
            AppMainAbout, 
            AppMainWhy,
            AppMainRecent,
        }
    }


</script>

<template>

    <AppMainAbout/>

    <AppMainWhy/>

    <AppMainRecent/>

</template>

<style lang="scss" scoped>

</style>