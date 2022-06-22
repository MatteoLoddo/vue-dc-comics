<template>
        <div class="container-img">
            <img :src="imgUrl" :alt="`immagine del fumetto ${comicType}`">
            <div>{{comicType}}</div>
        </div>
</template>

<script>
export default{

    props:{
        imgUrl: String,
        comicType: String,

    }

}
</script>

<style lang="scss">
.container-img{
    img{
        height:100%;
    }
}
</style>