<template>
    <div>
        <div class="container ">
            <div class="row">
                <div class="col-5 d-flex flex-wrap ">
                    <ul v-for="(items,i) in FooterLink" :key="i" class="d-flex flex-column">{{items.nameGroup}}
                        <li class="list-unstyled text-break" v-for="(link,i) in items.linkList" :key="i">
                            <a class="text-decoration-none p-1" href="#">{{link}}</a>
                        </li>
                    </ul>
                </div>
                <div class="col-7 dc-logo-jumbo">
                </div>
            </div>
        </div>
    </div>
</template>



<script>
export default{


    data() {
        return{
            FooterLink:[    
                {
                    nameGroup:"DC COMICS",
                    linkList:[
                        'Character',
                        'Comics',
                        'Movies',
                        'Tv',
                        'Games',
                        'Videos',
                        'News'
                    ]
                },
                {
                    nameGroup:"DC",
                    linkList:[
                        'Therms Of Use',
                        'Privacy Policy (New)',
                        'Ad Chose',
                        'Advertising',
                        'Jobs',
                        'Subscription',
                        'Talents Workshop',
                        'CPSC Certificates',
                        'Ratings',
                        'Shop Help',
                        'Contact Us',
                    ]
                },
                {
                    nameGroup:"SITES",
                    linkList:[
                        'DC',
                        'MAD Magazine',
                        'DC kids',
                        'DC Universe',
                        'DC Power Visa',
                    ]
                },
                {
                    nameGroup:"SHOP",
                    linkList:[
                        'Shop DC',
                        'Shop DC Collectibles',
                    ]
                },
            ]
        }
    }
}
</script>


<style lang="scss" scoped>

.jumbotron{
    color:#fff;
    background-image: url(/public/img/footer-bg.jpg);
}
.col-7{
    &.dc-logo-jumbo{
        background-image: url(/public/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-size: cover;
        background-position: 0px;  
        }
}
.col-5{
        
    ul{
        padding:0.8rem;
        li{
            a{
                color:#717171

            }
        }
    }
}
</style>