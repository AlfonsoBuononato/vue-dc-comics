<template>
    <footer>
        <div class="container-top-footer">
            <!-- CONTATTI -->
            <div class="contatti">
                <div class="info">
                    <div class="dc-comics" v-for="(title, index) in data" :key="index">
                        <h3>{{title.sottotitolo}}</h3>
                        <ul class="list-dc-comics">
                            <li v-for="(info, index) in title.infos" :key="index"><a href="#">{{info}}</a></li>
                        </ul>
                    </div>
                </div>
            </div>
            <img src="../assets/dc-logo-bg.png" alt="">
        </div>
        <div class="container-bottom">
            <!-- SOCIAL -->
            <div class="social">
                <div class="sign-up">
                    <div class="button">
                        <span>SIGN UP</span>
                    </div>
                </div>
                <div class="follow-uf">
                    <ul class="social">
                        <h5>FOLLOW US</h5>
                        <li v-for="(icon, index) in social" :key="index"><a href="#"><i :class="icon"></i></a></li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name:"Footer",
    data(){
        return {
            data:[
                {
                    sottotitolo: "DC COMICS",
                    infos: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"]
                },
                {
                    sottotitolo: "SHOP",
                    infos: ["Shop DC", "Shop DC Collectibles",]
                },
                {
                    sottotitolo: "DC COMICS",
                    infos: ["Terms Of Use", "Privacy policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help"]
                },
                {
                    sottotitolo: "DC COMICS",
                    infos: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"]
                }
            ],
            social:["fab fa-facebook", "fab fa-twitter", "fab fa-youtube","fab fa-pinterest", "fas fa-map-marker-alt"]
        }
    }
}
</script>

<style lang="scss">
    footer{
        height: 300px;
    }
    footer h3{
        color: #fff;
    }

    footer a{
        color: #424242;
    }
    /* CONTATTI */
    .container-top-footer{
        position: relative;
        background-image: url(../assets/footer-bg.jpg);
    }
    footer .contatti{
        max-width: 1200px;
        margin: auto;
    }

    .info{
        display: flex;
        padding: 30px 0;
    }

    .info .dc-comics{
        padding: 0 10px;
    }

    .info h3{
        margin-bottom: 10px;
    }

    .container-top-footer img{
        width: 400px;
        position: absolute;
        top: 0;
        right: 15%;
        transform: translate(0,-5%);
    }

    /* SOCIAL */
    .container-bottom{
        position: relative;
        background-color: #2f2f2f;
        z-index: 3;
    }
    footer .social{
        display: flex;
        justify-content: space-between;
        align-items: center;
        max-width: 1200px;
        height: 60px;
        margin: auto;
    }

    footer .social .button{
        padding: 5px;
        border: 1px solid #166fca;
        color: #fff;
    }

    footer{
        ul{
            a{
                font-size: 20px;
                padding: 5px;
            }
        }
    }
</style>