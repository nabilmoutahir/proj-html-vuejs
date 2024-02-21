<script>

    import { store } from '../store/store';

    export default {
        data() {

            return {

                store,

                title: 'Recent Work',

                view: 'VIEW ALL WORK',

                images:[
                    'portfolio1_featured_item-600x480.jpg',
                    'portfolio2_featured_item-1200x960.jpg',
                    'portfolio3_featured_item-1200x960.jpg',
                    'portfolio4_featured_item-1200x960.jpg',
                    'portfolio5_featured_item-1200x960.jpg',
                    'portfolio6_featured_item-1200x960.jpg'
                ]
            }

        },

    }

</script>

<template>
    <section class="text-white">
        <div class="section-top">
            <h2 class="overflow-hidden fs-1">
                {{ title }}
            </h2>

            <div>
                {{ store.services }}
            </div>
        </div>

        <div class="m-0 p-0">
            <div class="row d-flex flex-wrap">
                <div v-for="image in images" class="col-6 p-0">
                    <img :src="'/3portfolio/' + image" alt="">
                </div>
            </div>
        </div>

       <a href="">
            <div class="section-bot text-center py-5">
            
                {{ view }}
            
            </div>
       </a>


    </section>
</template>

<style lang="scss" scoped>

    

    section{
        .section-top{
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            padding: 100px 0;
            background-color: #87c856;
        }

        img{
            width: 100%;
            object-fit: cover;
        }

        .section-bot{
            background-color: #f9225b;
            font-size: smaller;
        }

        a {
            margin: 0;
            font-size: small;
            color: white;
            text-decoration: none;
        }

    }

</style>