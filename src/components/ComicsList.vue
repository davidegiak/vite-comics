<script>
export default {
    name: "ComicsList",
    props: ["comic"]
}
</script>

<template>
        <div class="col-2 flex-column comic-card">
            <div class="img-cont">
                <img :src="comic.thumb" alt="">
            </div>
            <h4> {{ comic.series }} </h4>
        </div>
</template>

<style scoped>
.comic-card{
}
img {
    width: 100%;
    height: 14rem;
}
h4 {
    font-size: 1rem;
}

.img-cont{
    width: 10rem;
    object-fit: contain;
}
</style>