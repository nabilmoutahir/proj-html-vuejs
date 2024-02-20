<script>

    export default {

        data() {
            return {
                headerButtons: [
                    {
                        link: 'link',
                        icon: 'icon'
                    },
                    {
                        link: 'link',
                        icon: 'icon'
                    }
                ],

                slogan:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde, modi!',

                headerLogo:'../assets/1logo/av-freelance-logo-retina.png'

            }
        },       



    }

</script>

<template>

    <header>
        <div class="d-flex justify-content-between py-4 px-5 mb-5">
            <div>
                <a href="#">
                    <img src="../assets/1logo/av-freelance-logo-retina.png" alt="">
                </a>
            </div>

            <div>
                <div>
                    EMOJI
                </div>

                <div>
                    EMOJI
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
                AVADA FREELANCE
            </div>

            <h1>
                Art Director
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
        background-image: url(../assets/2banner/banner_images.jpg);
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