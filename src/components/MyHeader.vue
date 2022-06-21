<template>
    <div class="">
        <div class=" container d-flex">
            <div class="p-2">
                <img src="/img/dc-logo.png" alt="">
            </div>

            <div class="flex-grow-1">
            </div>
            
                <ul class=" m-0 d-flex flex-grow-1 justify-content-end  ">
                    <li class="list-unstyled d-flex " v-for="(items,i) in NavBar" :key="i">
                        <a class="fs-8 fw-bold text-decoration-none p-2 align-self-center" href="#">{{items.title}}</a>
                    </li>
                </ul>
        </div>
    </div>
</template>

<script>
export default{
    name:"MyHeader",

    data() {
        return{
            NavBar:[
                {
                    title: "CHARACTER"
                },
                {
                    title: "COMICS"
                },
                {
                    title: "MOVIES"
                },
                {
                    title: "TV"
                },
                {
                    title: "GAMES"
                },
                {
                    title: "COLLECTIBLES"
                },
                {
                    title: "VIDEO"
                },
                {
                    title: "FANS"
                },
                {
                    title: "NEW"
                },
                {
                    title: "SHOP"
                },
            ],
        }
    }

}
</script>

<style lang="scss" scoped>
.fs-8{
    font-size:0.8rem;
    }

    ul{
        li{
            &:hover{
            border-bottom:2px solid blue;}
        }
    }





</style>