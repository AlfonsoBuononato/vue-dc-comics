<template>
    <main class="content">
        <div class="container-top">
            <!-- CONTENT TOP -->
            <!-- JUMBOTRON -->
                <div class="jumbotron">
                    <img src="../assets/jumbotron.jpg" alt="" style="width: 100%; height: 100%">
                </div>
            <!-- SEZIONE FUMETTI GESTITI JAVASCRIPT -->
            <div class="content-top">
                <div class="super-hero">
                    <!-- MINI TITLE POSITION ABSOLUTE -->
                    <div class="mini-titile">
                        <span>current series</span>
                    </div>
                    <!-- FUMETTI JAVASCRIPT -->
                    <div class="fumetti">
                        <div class="img" v-for="(hero, index) in superHero" :key="index">
                            <img :src="hero.thumb" alt="">
                            <h4>{{hero.series}}</h4>
                        </div>
                    </div>
                    <!-- BUTTON ALTRI FUMETTI -->
                    <div class="more">
                        <span>LOAD MORE</span>
                    </div>

                </div>
            </div>
        </div>
        <div class="container-bottom">
            <!-- CONTENT BOTTOM -->
            <div class="content-bottom">
                <ul>
                    <li v-for="(digital, index) in comicsDigital"
                        :key="index">
                        <a href="#"><img :src="digital.img" alt=""></a>
                        <span>{{digital.nome}}</span>
                    </li>
                </ul>
            </div>
        </div>
    </main>
</template>

<script>
export default {
    name:"Main",
    data(){
        return{
            comicsDigital: [
                {
                    img:require("../assets/buy-comics-digital-comics.png"),
                    nome: "DIGITAL COMICS",
                },
                {
                    img:require("../assets/buy-comics-merchandise.png"),
                    nome: "DIGITAL COMICS",
                },
                {
                    img:require("../assets/buy-comics-shop-locator.png"),
                    nome: "DIGITAL COMICS",
                },
                {
                    img:require("../assets/buy-comics-subscriptions.png"),
                    nome: "DIGITAL COMICS",
                },
                {
                    img:require("../assets/buy-dc-power-visa.svg"),
                    nome: "DIGITAL COMICS",
                },
            ],
            superHero:[
                {
                    thumb:'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX',
                    price: '$19.99',
                    series: 'Action Comics',
                    type: 'comic book',
                },
                {
                    thumb:'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01',
                    price: '$3.99',
                    series: 'American Vampire 1976',
                    type: 'comic book',
                },
                {
                    thumb:'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb',
                    price: '$16.99',
                    series: 'Aquaman',
                    type: 'graphic novel',
                },
                {
                    thumb:'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76',
                    price: '$2.99',
                    series: 'Batgirl',
                    type: 'comic book',
                },
                {
                    thumb:'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
                    price: '$3.99',
                    series: 'Batman',
                    type: 'comic book',
                },
                {
                    thumb:'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
                    price: '$2.99',
                    series: 'Batman Beyond',
                    type: 'comic book',
                },
                {
                    thumb:'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8',
                    price: '$3.99',
                    series: 'Batman/Superman',
                    type: 'comic book',
                },
                {
                    thumb:'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk',
                    price: '$4.99',
                    series: 'Batman/Superman Annual',
                    type: 'comic book',
                },
                {
                    thumb:'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8',
                    price: '$5.99',
                    series: 'Batman: The Joker War Zone',
                    type: 'comic book',
                },
                {
                    thumb:'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY',
                    price: '$6.99',
                    series: 'Batman: Three Jokers',
                    type: 'comic book',
                },
                {
                    thumb:'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX',
                    price: '$4.99',
                    series: 'Batman: White Knight Presents: Harley Quinn',
                    type: 'comic book',
                },
                {
                    thumb:'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq',
                    price: '$16.99',
                    series: 'Catwoman',
                    type: 'graphic novel',
                },
]

        }
    }
}
</script>

<style scoped lang="scss">
    /* STYLE PER LE IMMAGINI */
    @import "../style/style-img-hero.scss";

    .content{
        color: white;
    }
    /* CONTENT TOP */
    .container-top{
        background-color: #000;
    }
    .content .content-top{
        max-width: 1200px;
        margin: auto;
        font-size: 1.2rem;
    }
    /* CONTENT BOTTOM */
    .container-bottom{
        background-color: #0f82f7;
    }
    .content .content-bottom{
        display: flex;
        align-items: center;
        max-width: 1200px;
        height: 100px;
        margin: auto;
    }
    .content .content-bottom ul{
        display: flex;
    }
    .content .content-bottom li{
        display: flex;
        align-items: center;
    }
    .content .content-bottom img{
        width: 50px;
    }
</style>