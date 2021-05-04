<template>
    <main class="content">
        <div class="container-top">
            <!-- CONTENT TOP -->
            <div class="content-top">
                <span>Content goes here</span>
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
            ]
        }
    }
}
</script>

<style scoped>
    .content{
        color: white;
    }
    /* CONTENT TOP */
    .container-top{
        background-color: #000;
    }
    .content .content-top{
        max-width: 1200px;
        height: 100px;
        margin: auto;
        font-size: 1.2rem;
        line-height: 100px;
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