<script>
export default {
    name:"SingleComic",
    props: ["card"],
    components: {
    },
}
</script>

<template>
    <div class="comic-card col-2 d-flex flex-column justify-content-center align-items-center">
        <div class="img-cont">
            <img :src="card.thumb" alt="">
        </div>
        <h4> {{ card.series }} </h4>
    </div>
</template>

<style scoped>
img {
    width: 100%;
    height: 14rem;
}

.img-cont {
    width: 10rem;
}

h4 {
    font-size: 1rem;

}
</style>