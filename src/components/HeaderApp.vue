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
        },
        methods: {
            blueBarsFunction() {
                let bar = document.querySelector(".myBlueLinksBar");
                let link = document.querySelector("a")
                if (bar.classList.contains("d-none")) {
                    bar.classList.replace("d-none", "d-block")
                    a.classList.add("text-blue")
                }
            },
            blueBarsFunctionLeave() {
                let bar = document.querySelector(".myBlueLinksBar");
                if (bar.classList.contains("d-block")) {
                    bar.classList.replace("d-block", "d-none")
                }
            }
        }
    } 
</script>

<template>
    <header class="">
        <div class="myContainer d-flex justify-content-center align-items-center justify-content-around">
            <div class="logo-cont d-flex justify-content-center">
                <img class="my-2" src="/dc-logo.png" alt="">
            </div>
            <div class="links-cont d-flex">
                <ul class="d-flex ">
                    <li v-for="link, i in links">
                        <a @mouseover="blueBarsFunction()" @mouseleave="blueBarsFunctionLeave()" class="mx-2 d-flex flex-column" :href="link.url">
                            {{ link.text }}
                        </a>
                        <div class="d-none myBlueLinksBar"></div>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style scoped>
    header{
        background-color: white;
        position: fixed;
        width: 100%;
    }
    img {
        width: 100%;
        object-fit: contain;
    }
    .logo-cont {
        width: 6rem;
    }
    a {
        text-decoration: none;
        color: black;
    }
    .myBlueLinksBar {
        width: 100%;
        height: 5px;
        background-color: #0282f9;
    }
    ul {
        list-style: none;
    }


    
</style>