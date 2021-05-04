<template>
    <footer>
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
       <!-- SOCIAL -->
       <div class="social">
           <div class="sign-up">
               ciao
           </div>
           <div class="follow-uf">
               ciao
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

    footer .contatti{
        display: flex;
        background-image: url(../assets/footer-bg.jpg);
        
    }
</style>