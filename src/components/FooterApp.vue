<script>
    export default {
        data() {
            return {
                footLinks:[
                    {
                        text: "DIGITAL COMICS",
                        url: "#",
                        img: ("../assets/img/buy-comics-digital-comics.png")
                    },
                    {
                        text: "DC MERCHANDISE",
                        url: "#",
                        img: "../assets/img/buy-comics-merchandise.png"
                    },
                    {
                        text: "SUBSCRIPTION",
                        url: "#",
                        img: "../assets/img/buy-comics-shop-locator.png"
                    },
                    {
                        text: "COMIC SHOP LOCATOR",
                        url: "#",
                        img: "../assets/img/buy-comics-subscriptions.png"
                    },
                    {
                        text: "DC POWER VISA",
                        url: "#",
                        img: "../assets/img/buy-dc-power-visa.svg"
                    },
                ]
            }
        }
    }
</script>

<template>
    <footer>
        <section class="blue-section d-flex justify-content-around">
            <div v-for="link in footLinks" class="mycard">
                <div class="img-card-cont">
                    <img :src="link.img" alt="">
                </div>
                <a :href="link.url"> {{ link.text }} </a>
            </div>
        </section>
    </footer>
</template>

<style scoped>
    .blue-section {
        background-color: #0282f9;
        height: 5rem;
    }
</style>