<script>

import { store } from '../store/store';

export default {
    data() {

        return {

            store,

            title:'Expert Design Advice',

            subTitle:'TRENDING DESIGN NEWS',


          
            medias:[
                'blog3-featured-800x533.jpg',
                'blog2-featured-800x533.jpg',
                'blog1-featured-800x533.jpg',
            ],

            texts: [
            'Live The Design Process',
            "What's Next of The App Store?",
            'The Humble Wooden Desk'
        ]


           
        }

    },

}

</script>

<template>
    <section>
        <div class="title-section text-center text-white py-5">
            <h2 class="overflow-hidden pt-5">
                {{ title }}
            </h2>

            <h6 class="pt-3">
                {{ subTitle }}
            </h6>
        </div>

        <div class="article-section d-flex align-content-center">
            <div v-for="(media, index) in medias">
                <a href="#">
                    <div>
                        <img :src="'public/5advice/' + media" alt="">
                    </div>

                    <div>
                        <h3 class="title-article pt-3 overflow-hidden">
                            {{ texts[index] }}
                        </h3>

                        <div class="text-article pb-5">
                            {{ store.shortText }}
                        </div>
                    </div>
                </a>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>

    section{
        
        .title-section {
            background-color: #49629b;
        }

        img{
            width: 100%;
        }

        a{
            text-decoration: none;
        }

        .article-section{
            background-color: #191c23;
            
        }

        .title-article{
            color: #fa225b;
        }

        .text-article{
            color: #7a89ab;
        }
    }

</style>