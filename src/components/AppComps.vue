<script>
    import AppHeader from './AppHeader.vue';

    export default {
        data () {
            return{
                headerItem: 
                        {
                            img: '/1logo/av-freelance-logo-retina.png',
                            url: '#',
                            icon: 'icon',
                            name:'AVADA FREELANCE',
                            title:'Art Director',
                            slogan: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde, modi!'
                        }
                    
            }
            
        },

        components: {
            AppHeader
        }

    }
</script>

<template>

    <AppHeader 
    :img="headerItem.img" 
    :url="headerItem.url"
    :icon="headerItem.icon"
    :name="headerItem.name"
    :title="headerItem.title"
    :slogan="headerItem.slogan"
    />
    



</template>

<style lang="scss" scoped>
</style>