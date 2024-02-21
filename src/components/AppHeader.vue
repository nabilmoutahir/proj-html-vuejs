<script>
    
    export default { 

        // PROPS
        props: {
            img: String,
            url: String,
            icon: String,
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
                <div>
                    {{ icon }}
                </div>

                <div>
                    {{ icon }}
                </div>
            </div>
        </div>
    
        <div>
            <div>
                <div>
                    SQUARE
                </div>

                <div>
                   SQUARE 
                </div>
            </div>
        </div>

        <div class="text-center mt-5 py-5">
            <div>
                {{ name }}
            </div>

            <h1 class="overflow-hidden">
                {{ title }}
            </h1>

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