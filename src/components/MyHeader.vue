<template>
    <div>
        <div class="container d-flex align-items-center p-2">
            <div class="">
                <img src="/img/dc-logo.png" alt="">
            </div>

            <div class="flex-grow-1">
            </div>
            
            <div class="">
                <ul class="flex-grow justify-content-end d-flex">
                    <li class="list-unstyled" v-for="(items,i) in NavBar" :key="i">
                        <a class="p-2" href="#">{{items.title}}</a>
                    </li>
                </ul>
            </div>
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

</style>