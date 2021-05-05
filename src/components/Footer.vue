<template>
    <footer>
        <div class="container-top-footer">
            <!-- CONTATTI -->
            <div class="contatti">
                <div class="info-1">
                    <div class="dc-comics">
                        <ul class="list-dc-comics" v-for="(title, index) in data" :key="index">
                            <h3>{{title.sottotitolo}}</h3>
                            <li><a href="#">{{title.info}}</a></li>
                        </ul>
                    </div>
                </div>
            </div>
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
                        <li><i class="fab fa-facebook"></i></li>
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
                    info: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"]
                },
                {
                    sottotitolo: "SHOP",
                    info: ["Shop DC", "Shop DC Collectibles",]
                },
                {
                    sottotitolo: "DC COMICS",
                    info: ["Terms Of Use", "Privacy policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help"]
                },
                {
                    sottotitolo: "DC COMICS",
                    info: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News" ]
                }
            ]
        }
    }
}
</script>

<style>
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
        background-image: url(../assets/footer-bg.jpg);
    }
    footer .contatti{
        display: flex;
        max-width: 1200px;
        margin: auto;
    }

    /* SOCIAL */
    .container-bottom{
        background-color: #2f2f2f;
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
</style>