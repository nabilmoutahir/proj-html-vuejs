<script>

import { store } from '../store/store';

export default {
    data() {

        return {

            store,

            title: 'Recent Work',

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
        <div class="section-top text-center">
            <h2>
                {{ title }}
            </h2>

            <div>
                {{ store.services }}
            </div>
        </div>

        <div>
            <div class="row d-flex flex-wrap">
                <div v-for="image in images" class="col-6 p-0">
                    <img :src="'/3portfolio/' + image" alt="">
                </div>
            </div>
        </div>

        <div class="section-bot">
            <a href="#">
                VIEW ALL WORK
            </a>
        </div>


    </section>
</template>

<style lang="scss" scoped>

    

    section{
        .section-top{
            background-color: #87c856;
        }

        img{
            width: 100%;
            object-fit: cover;
        }

        .section-bot{
            background-color: #f9225b;
        }

        a {
            color: white;
            text-decoration: none;
        }

    }

</style>