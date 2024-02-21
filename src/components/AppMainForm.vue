<script>

    import { store } from '../store/store';

    export default {
        data() {

            return {

                store,

                title:"Let's Work Togheter",

                subTitle:'TELL ME MORE ABOUT YOUR PROJECT',

            }

        },

    }

</script>

<template>
    <section>
        <div class="text-center py-5">
            <h2 class="overflow-hidden py-3 pt-5">
                {{ title }}
            </h2>

            <h6 class="pb-5">
                {{ subTitle }}
            </h6>

            <p>
                {{ store.shortText }}
            </p>
        </div>

        

        <div class="d-flex justify-content-center align-content-center pb-5">
            <div class="form-section col-4">
                <input type="text" class="form-control my-3 py-3" placeholder="NAME*">
                <input type="text" class="form-control my-3 py-3" placeholder="EMAIL*">
                <input type="text" class="form-control my-3 py-3" placeholder="PHONE">
                <button class="btn btn-danger my-3 py-3 fs-5" type="button">LET'S TALK</button>
            </div>
        </div>

        
    </section>
</template>

<style lang="scss" scoped>

    section{
        background-color: #ebeced;

        button{
            width: 100%;
        }
        
        h6, p{
            font-weight: normal;
            color: #7b83b0;
        }

    }

</style>