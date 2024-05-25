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
    <div class="jumbo"></div>
    <div>
        <ComicsList/>
    </div>
</template>

<style scoped>
.jumbo {
    background-image: url(/public/jumbotron.jpg);
    height: 20rem;
}
</style>