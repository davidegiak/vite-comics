<script>
    export default {
        data() {
            return {
                footLinks:[
                    {
                        text: "DIGITAL COMICS",
                        url: "#",
                        img: "/buy-comics-digital-comics.png"
                    },
                    {
                        text: "DC MERCHANDISE",
                        url: "#",
                        img: "/buy-comics-merchandise.png"
                    },
                    {
                        text: "SUBSCRIPTION",
                        url: "#",
                        img: "/buy-comics-shop-locator.png"
                    },
                    {
                        text: "COMIC SHOP LOCATOR",
                        url: "#",
                        img: "/buy-comics-subscriptions.png"
                    },
                    {
                        text: "DC POWER VISA",
                        url: "#",
                        img: "/buy-dc-power-visa.svg"
                    },
                ],
                socials:[
                    { img: "/footer-facebook.png" },
                    { img: "/footer-periscope.png" },
                    { img: "/footer-pinterest.png" },
                    { img: "/footer-twitter.png" },
                    { img: "/footer-youtube.png" }
                ],
                dcComicsFootLinks:[
                    {link: "Characters"},
                    {link: "Comics"},
                    {link: "Movies"},
                    {link: "TV"},
                    {link: "Games"},
                    {link: "videos"},
                    {link: "News"},
                ],
                shopFootLinks:[
                    {link: "Shop Dc"},
                    {link: "Shop Dc Collectible"}
                ],
                dcFootLinks:[
                    {link: "Terms of use"},
                    {link: "Privacy policy(New)"},
                    {link: "Ad Choices"},
                    {link: "Advertising"},
                    {link: "Jobs"},
                    {link: "Subscriptions"},
                    {link: "Talent Workshop"},
                    {link: "CPSC Certificates"},
                    {link: "Ratings"},
                    {link: "Shop Help"},
                    {link: "Contact Us"}
                ],
                sitesFootLinks:[
                    {link: "DC"},
                    {link: "MAD Magazine"},
                    {link: "DC Kids"},
                    {link: "DC Univers"},
                    {link: "DC Power Visa"}
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
            <div class="myContainer d-flex">
                <div class="col-2 d-flex flex-column">
                    <ul>
                        <li><h3> DC COMICS </h3></li>
                        <li v-for="element in dcComicsFootLinks"><a class="middle-foot-links" href="#"> {{ element.link }} </a></li>
                    </ul>
                    <ul>
                        <li><h3>SHOP</h3></li>
                        <li v-for="element in shopFootLinks">
                            <a class="middle-foot-links" href="#"> {{ element.link }} </a>
                        </li>
                    </ul>
                </div>
                <div class="col-2 d-flex flex column">
                    <ul>
                        <li><h3>DC</h3></li>
                        <li v-for="link in dcFootLinks"><a class="middle-foot-links" href="#"> {{ link.link }} </a></li>
                    </ul>
                </div>
                <div class="col-2 d-flex flex column">
                    <ul>
                        <li><h3>SITES</h3></li>
                        <li v-for="link in sitesFootLinks"><a class="middle-foot-links" href="#"> {{ link.link }} </a></li>
                    </ul>
                </div>
                <div class="dc-back-cont">
                    <!-- <img class="dc-back" src="../../public/dc-logo-bg.png" alt=""> -->
                </div>
            </div>
        </section>
        <section class="pageFoot py-3">
            <div class="myContainer d-flex justify-content-between">
                <div class="btn-cont d-flex align-items-center">
                    <button type="button" class="btn btn-outline-primary">SIGN-UP NOW!</button>
                </div>
                <div class="socials-cont d-flex gap-2 justify-content-center align-items-center">
                    <h4 id="followUs">FOLLOW US</h4>
                    <div class="social-icon-cont d-flex gap-3">
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
        background-image: url(../../public/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }
    .pageFoot {
        background-color: #222;
    }
    .socials {
        width: 2rem;
    }
    #followUs {
        color: #0282f9;
        font-weight: 1000;
    }
    li {
        list-style: none;
    }
    .dc-back {
        object-fit: cover;
    }
    .dc-back-cont {
        background-image: url(/public/dc-logo-bg.png);
        background-size: cover;
        background-position: center;
        width: 40rem;
        margin-left: 5rem;
    }
    ul {
        margin-top: 2rem;
    }
    .middle-foot-links {
        text-decoration: none;
        color: white;
        opacity: 0.4;
    }
    .middle-foot-links:hover {
        transition: 0.5s;
        opacity: 1;
    }
</style>