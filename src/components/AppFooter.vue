<script>

    export default {

        props:{
            img: String,
            url: String,
            socials:String,
        },



    };

</script>

<template>

    <footer>
        <section class="py-5">

            <div class="text-center pt-5">
                <a :href="url">
                    <img :src="img" alt="">
                </a>
            </div>

            <div class="text-center py-4">
                <span>Copyright 2012 - 2020 |</span>
                <span> Avada Theme by <a :href="url">Theme Fusion</a> |</span>
                <span> All Rights Reserved |</span>
                <span> Powered by <a :href="url">WordPress</a></span>
            </div>

            <div class="d-flex justify-content-center align-content-center pb-5">
                <div class="px-3" v-for="social in socials">
                    <a :href="url">
                        <i :class="social"></i>
                    </a>
                </div>
            </div>

        </section>
    </footer>

</template>

<style lang="scss" scoped>

    
    footer{
        background-color: #1d2028;
        color: #7887a9;
        
        a{
            color: white;
            text-decoration: none;
        }

        i{
            color: white;
            overflow: hidden;
            font-size: xx-large;
        }
    }

</style>