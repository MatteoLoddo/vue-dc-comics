<template>
    <div>
        <div class="">
            <div class="row w-50">
                <div class="col-4 p-1" v-for="(items,i) in FooterLink" :key="i">
                    <ul class="d-flex flex-column ">{{items.nameGroup}}
                        <li class="list-unstyled text-break" v-for="(link,i) in items.linkList" :key="i">
                            <a class="p-1" href="#">{{link}}</a>
                        </li>
                    </ul>
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
</style>