<script>

    import AppFooter from './AppFooter.vue';

export default {

    data (){
        return{
            footerItem: {
                img:'/1logo/avada-footer-logo.png',
                url:'#',
            },

            socials:[
                'fa-brands fa-square-facebook',
                'fa-brands fa-square-twitter',
                'fa-brands fa-square-instagram',
                'fa-brands fa-square-youtube'
            ],

        }

    },

    components: {
        AppFooter
    }

};

</script>

<template>

    <app-footer
        :img="footerItem.img"
        :url="footerItem.url"
        :socials="socials"
    
    />

</template>

<style lang="scss" scoped>



</style>