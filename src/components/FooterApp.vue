<script>
    export default {
        data() {
            return {
                footLinks:[
                    {
                        text: "DIGITAL COMICS",
                        url: "#",
                        img: "./buy-comics-digital-comics.png"
                    },
                    {
                        text: "DC MERCHANDISE",
                        url: "#",
                        img: "./buy-comics-merchandise.png"
                    },
                    {
                        text: "SUBSCRIPTION",
                        url: "#",
                        img: "./buy-comics-shop-locator.png"
                    },
                    {
                        text: "COMIC SHOP LOCATOR",
                        url: "#",
                        img: "./buy-comics-subscriptions.png"
                    },
                    {
                        text: "DC POWER VISA",
                        url: "#",
                        img: "./buy-dc-power-visa.svg"
                    },
                ],
                socials:[
                    { img: "./footer-facebook.png" },
                    { img: "./footer-periscope.png" },
                    { img: "./footer-pinterest.png" },
                    { img: "./footer-twitter.png" },
                    { img: "./footer-youtube.png" }
                ]
            }
        }
    }
</script>

<template>
    <footer>
        <section class="blue-section">
            <div class="myContainer d-flex justify-content-around justify-content-center align-items-center gap-3">
                <div v-for="link in footLinks" class="mycard d-flex gap-1">
                    <div class="img-card-cont my-3">
                        <img class="links-img" :src="link.img" alt="">
                    </div>
                    <div class="links-cont d-flex justify-content-center align-items-center">
                        <a class="text-white text-decoration-none" :href="link.url"> {{ link.text }} </a>
                    </div>
                </div>
            </div>
        </section>
        <section class="middleFoot">
            
        </section>
        <section class="pageFoot">
            <div class="myContainer d-flex justify-content-between">
                <div class="btn-cont vertical-align-middle">
                    <button type="button" class="btn btn-outline-primary">SIGN-UP NOW!</button>
                </div>
                <div class="socials-cont d-flex gap-2 justify-content-center align-items-center">
                    <h4 id="followUs">FOLLOW US</h4>
                    <div class="d-flex gap-3">
                        <img v-for="element in socials" class="socials" :src="element.img" alt="">
                    </div>
                </div>
            </div>
        </section>
    </footer>
</template>

<style scoped>
    .blue-section {
        background-color: #0282f9;
        height: 15vh;
    }
    .img-card-cont {
        width: 4rem;
    }
    .links-img {
        width: 100%;
        height: 3rem;
        object-fit: contain;
    }
    .middleFoot {
        height: 45vh;
        background-image: url(../../public/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }
    .pageFoot {
        background-color: #222;
        height: 10vh;
    }
    .socials {
        width: 100%;
    }
    #followUs {
        color: #0282f9;
    }
</style>