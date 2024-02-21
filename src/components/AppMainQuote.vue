<script>

import { store } from '../store/store';

export default {

    data() {

        return {

            store,

            quoteImg: 'quotes-1.png',

            quote: "That's been my mantras - focus and semplicity. Simple can be harder than complex; you have to work hard to get your thinking clean to make it simple",

            subQuote: 'STEVE JOBS - APPLE',

            brandTitle: 'TRUSTED BY GLOBAL BRANDS',

            brandIcons: [
                'logo_demo_1.png',
                'logo_demo4.png',
                'Vector_Smart_Object-1.png',
                'Vector_Smart_Object-2.png',
                'Vector_Smart_Object.png'
            ]

        }

    }
}

</script>

<template>
    <section class="text-white">

        <div class="text-center py-5">
            <div class="py-5">
                <img :src="'public/4quotes-brands/' + quoteImg" alt="">
            </div>

            <div class="pb-3 fst-italic">
                "{{ quote }}"
            </div>

            <div class="pb-5 fw-bold">
                {{ subQuote }}
            </div>
        </div>

        <div class="text-center pb-5">
            <div class="fw-bold">
                {{ brandTitle }}
            </div>

            <div class="d-flex justify-content-center align-content-center py-5">
                <div class="px-5" v-for="icon in brandIcons">
                    <a href="">
                         <img :src="'public/4quotes-brands/' + icon" alt="">
                    </a>   
                </div>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>

    section{
        background-image: url(public/4quotes-brands/testimonial_bkgd.jpg);
    }

</style>