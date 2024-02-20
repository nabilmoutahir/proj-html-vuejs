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

                slogan:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Unde, modi!'

            }
        },       



    }

</script>

<template>

    <header>
        <div class="d-flex justify-content-between py-2 px-5">
            <div>
                LOGO
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

        <div class="text-center">
            <div>
                AVADA FREELANCE
            </div>

            <div>
                ART DIRECTOR
            </div>

            <div>
                {{ slogan }}
            </div>
        </div>

    </header>

</template>

<style lang="scss" scoped>

    header{
        height: 100vh;
    }

</style>