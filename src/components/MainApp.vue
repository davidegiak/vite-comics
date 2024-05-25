<script>
import ComicsList from "./ComicsList.vue";

export default {
    components: {
        ComicsList
    },
    data(){
      
    }
}
</script>

<template>
    <div class="jumbo">
        <div class="myContainer d-flex align-items-end">
            <span class="badge text-bg-primary py-2 px-3">CURRIENT SERIES</span>
        </div>
    </div>
    <div>
        <ComicsList/>
    </div>
</template>

<style scoped>
.jumbo {
    background-image: url(/public/jumbotron.jpg);
    height: 20rem;
    background-size: cover;
}
.myContainer{
    height: 100%;
}
span{
    transform: translateY(10px);
}
</style>