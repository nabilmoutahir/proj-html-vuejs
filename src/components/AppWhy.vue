<script>

    import { store } from '../store/store';

    export default {
        data (){

            return {

                store,

                title: 'Why Work With Me',

                icons: {
                    web: 'fa-solid fa-shield-cat',
                    brand: 'fa-solid fa-shield-halved',
                    ui: 'fa-regular fa-gem'
                },

                services: {
                    web: 'Web Design',
                    brand: 'Branding',
                    ui: 'UX/UI'
                },

            }


        }
    }
</script>

<template>
    <section>

        <div class="section-container py-5">
            <div class="text-center py-3">
                <h2 class="text-white">
                    {{ title }}
                </h2>

                <div class="sub-title">
                    {{ store.services }}
                </div>

                <p class="py-5">
                    {{ store.shortText }}
                </p>
            </div>

            <div class="text-white d-flex justify-content-center align-items-center">
                <div class="mx-5">
                    <div class="circle d-flex justify-content-center align-items-center">
                        <i :class="icons.web" href=""></i>
                    </div>

                    <div class="text-center py-3">
                        {{ services.web }}
                    </div>
                </div>

                <div class="mx-5">
                    <div class="circle d-flex justify-content-center align-items-center">
                        <i :class="icons.brand" href=""></i>
                    </div>

                    <div class="text-center py-3">
                        {{ services.brand }}
                    </div>
                </div>

                <div class="mx-5">
                    <div class="circle d-flex justify-content-center align-items-center">
                        <i :class="icons.ui" href=""></i>
                    </div>

                    <div class="text-center py-3">
                        {{ services.ui }}
                    </div>
                </div>
            </div>

            
        </div>


        
    </section>
</template>

<style lang="scss" scoped>

    section{

        background-color: #191c23;

        clip-path: polygon();

        .sub-title{
            color: #667290;
        }

        p{
            width: 30%;
            margin: auto;
            color: #3d6dab
        }

        i{
            color: #7a89ab;
            font-size: 50px;
        }
        .circle{
            border: 5px solid #fa225b;
            border-radius: 50%;
            height: 100px;
            aspect-ratio: 1;
        }
    }

</style>