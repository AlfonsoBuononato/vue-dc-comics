<template>
    <main class="content">
        <!-- CONTENT TOP -->
        <div class="content-top">
            <span>Content goes here</span>
        </div>
        <!-- CONTENT BOTTOM -->
        <div class="content-bottom">
            <ul>
                <li>
                    <a href="#"><img src="../assets/buy-comics-digital-comics.png" alt=""></a>
                    <span>Digital Comics</span>
                </li>
            </ul>
        </div>
    </main>
</template>

<script>
export default {
    name:"Main",
}
</script>

<style scoped>
    .content{
        color: white;
    }
    /* CONTENT TOP */
    .content .content-top{
        height: 100px;
        font-size: 1.2rem;
        line-height: 100px;
        background-color: #000;
    }
    /* CONTENT BOTTOM */
    .content .content-bottom{
        display: flex;
        align-items: center;
        height: 100px;
        background-color: #0f82f7;
    }
    .content .content-bottom li{
        display: flex;
        align-items: center;
    }
    .content .content-bottom img{
        width: 50px;
    }
</style>