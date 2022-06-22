<template>
    <div class="content">
    
        <div class="container pt-10">
            <ComicsList></ComicsList>
        </div>
    </div>
</template>


<script>
import ComicsList from '../components/ComicsList.vue';

export default{
    components:{ComicsList,}
    
}
</script>

<style lang ="scss" scoped>

.content{
    background-color: #1C1C1C;
    min-height:350px;

    .pt-10{
        color:#fff;
        padding-top:10rem;
    }
}


</style>