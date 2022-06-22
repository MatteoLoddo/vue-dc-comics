<template>
    <div class="content">
        <JumbotronComic class="mb-4 mt-7"></JumbotronComic>
        <div class="container">
            <ComicsList class=""></ComicsList>
        </div>
    </div>
</template>


<script>
import ComicsList from '../components/ComicsList.vue';
import JumbotronComic from '../components/JumbotronComic.vue'

export default{
    components:{ComicsList,JumbotronComic,}
    
}
</script>

<style lang ="scss" scoped>

.content{
    background-color: #1C1C1C;
    min-height:350px;
    color:#fff;
}

.mt-7{
    margin-top:7.5rem;
}


</style>