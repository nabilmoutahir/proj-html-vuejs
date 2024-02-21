<script>
    
    export default { 

        // PROPS
        props: {
            img: String,
            url: String,
            cross: String,
            menu: String,
            name: String,
            title: String,
            slogan: String,
            },
    };
</script>

<template>

    <header>
        <div class="d-flex justify-content-between py-4 px-5 mb-5">
            <div>
                <a :href="url">
                    <img :src="img" alt="">
                </a>
            </div>

            <div class="d-flex align-items-center">
                <a class="px-3" href="">
                    <div :class="cross">
                    </div>
                </a>

                <a class="px-3" href="">
                    <div :class="menu">
                    </div>
                </a>
            </div>
        </div>
    
        <!-- <div>
            <div>
                <div>
                    <a href="">
                        <div class="square1 m-2 rounded">
                    
                        </div>
                    </a>
                </div>
                
                <div>
                    <a href="">
                        <div class="square2 m-2 rounded">
                
                        </div>
                    </a>
                </div>
            </div>
        </div> -->

        <div class="text-center mt-5 py-5">
            <div>
                {{ name }}
            </div>

            <a href="">
                <h1 class="overflow-hidden">
                    {{ title }}
                </h1>
            </a>

            <div class="slogan">
                {{ slogan }}
            </div>
        </div>

    </header>

</template>

<style lang="scss" scoped>

    header{
        height: 100vh;
        background-color: black;
        background-image: url(/2banner/banner_images.jpg);
        background-size: cover;
        color: white;
        font-size: small;

        // .square1{
        //     right: 20px;
        // }

        // .square2 {
        //     top: 180px;
        //     right: 20px;
        // }
        // .square1, .square2{
        //     height: 50px;
        //     aspect-ratio: 1;
        //     background-color: white;
        //     position: fixed;
        //     z-index: 1;
        // }

        a{
            text-decoration: none;
            color: white;
        }

        img{
            height: 40px;
        }

        h1{
            font-size: 5rem;
            color: #FA225B;
        }

        .slogan{
            color: #667290;
        }
    }

</style>