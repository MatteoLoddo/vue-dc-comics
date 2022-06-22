<template>
    <ul class="d-flex justify-content-center">
        <li class="list-unstyled p-3" v-for="link in buyElement" :key="link.text">
        <img :src="link.img" alt="immagine DC merch">
        <span>{{link.text}}</span>
        </li>
    </ul>
</template>

<script>
export default{


data() {
    return{
        buyElement:[
            {
                text:"DIGITAL COMICS",
                img: "img/buy-comics-digital-comics.png"
            },
            {
                text:"DC MERCHANDISE",
                img: "img/buy-comics-merchandise.png"
            },
            {
                text:"COMIC SHOP LOCATOR",
                img: "img/buy-comics-shop-locator.png"
            },
            {
                text:"SUBSCRIPTION",
                img: "img/buy-comics-subscriptions.png"
            },
            {
                text:"DC POWER VISA ",
                img: "img/buy-dc-power-visa.svg"
            },
        ]
    }
}
}


</script>

<style lang="scss" scoped>
ul{
    padding: 1rem 0 1rem 0;
    margin: 0;
    background-color:#0C7CEC;
    li{
        img{
            height: 70px;
            padding: 0.5rem;
        }
        span{
            font-size:0.8rem;
            font-weight: bold;
            color: #ffff;

        }
    }
}
</style>