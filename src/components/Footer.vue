<template>
    <footer>
        <div class="container-top-footer">
            <!-- CONTATTI -->
            <div class="contatti">
                <div class="info-1">
                    <div class="dc-comics">
                        <ul class="list-dc-comics">
                            <h3>DC Comics</h3>
                            <li><a href="#">characters</a></li>
                        </ul>
                    </div>
                    <div class="shop">
                        <ul class="list-shop">
                            <h3>SHOP</h3>
                            <li><a href="#">Shop dc</a></li>
                        </ul>
                    </div>
                </div>
                <div class="info-2">
                    <div class="dc">
                        <ul class="list-dc">
                            <h3>DC</h3>
                            <li><a href="#">term of us</a></li>
                        </ul>
                    </div>
                </div>
                <div class="info-3">
                    <div class="sites">
                        <ul class="list-sites">
                            <h3>SITES</h3>
                            <li><a href="#">dc</a></li>
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
                        <li></li>
                        <li></li>
                        <li></li>
                        <li></li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name:"Footer",
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