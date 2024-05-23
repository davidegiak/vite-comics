<script>
    export default {
        data() {
            return {
                links:[
                    {
                        text: "CHARACTERS",
                        url: "#"
                    },
                    {
                        text: "COMICS",
                        url: "#"
                    },
                    {
                        text: "MOVIES",
                        url: "#"
                    },
                    {
                        text: "TV",
                        url: "#"
                    },
                    {
                        text: "GAMES",
                        url: "#"
                    },
                    {
                        text: "COLLECTIBLES",
                        url: "#"
                    },
                    {
                        text: "VIDEOS",
                        url: "#"
                    },
                    {
                        text: "FANS",
                        url: "#"
                    },
                    {
                        text: "NEWS",
                        url: "#"
                    },
                    {
                        text: "SHOP",
                        url: "#"
                    }
                ]
            }
        }
    }
</script>

<template>
    <header class="">
        <div class="myContainer d-flex justify-content-center align-items-center justify-content-around">
            <div class="logo-cont d-flex justify-content-center">
                <img class="my-2" src="../../public/dc-logo.png" alt="">
            </div>
            <div class="links-cont">
                <a class="mx-2" v-for="link in links" :href="link.url">{{ link.text }}</a>
            </div>
        </div>
    </header>
</template>

<style scoped>
    header{
        background-color: white;
        height: 15vh;
    }
    img {
        width: 100%;
        object-fit: contain;
    }
    .logo-cont {
        width: 6rem;
    }
</style>