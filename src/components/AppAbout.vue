<script>

    import { store } from '../store/store';

    export default {
        data() {

            return {

                store,

                title:"About Me",

                job:"UI & UX EXPERT",

            }

        },

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
                    {{ job }}
                </div>
            </div>

            <div class="row d-flex justify-content-center py-3">
                <div class="col-3">
                    <p>
                        {{ store.shortText }}
                    </p>

                    <p>
                        {{ store.longText }}
                    </p>
                </div>

                <div class="col-3">
                    <p>
                        {{ store.longText }}   
                    </p>

                    <p>
                        {{ store.shortText }}
                    </p>
                </div>
            </div>
        </div>

    </section>
</template>

<style lang="scss" scoped>

    section{

        background-color: #191c23;

        .section-container{
            background-color: #20232c;
            clip-path: polygon(0 0, 100% 0, 100% 100%, 0 85%);
        }

        .sub-title{
            color: #667290;
        }

        p {
            color: #3d6dab;
        }
    }

</style>