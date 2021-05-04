<template>
    <header>
        <!-- HEADER LEFT LOGO -->
        <div class="left">
            <img src="../assets/dc-logo.png" alt="">
        </div>
        <!-- HEADER RIGHT LOGO -->
        <div class="right">
            <ul class="list-item">
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
                <li>ciao</li>
            </ul>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
}
</script>

<style scoped>

    header{
        display: flex;
        align-items: center;
    }
    /* HEADER LEFT */
    .left{
        width: 50%;
        padding: 10px 20px;
    }

    .left img{
        width: 80px;
    }

    /* HEADER RIGHT */

    .right{
        width: 50%;
    }

    .list-item{
        width: 100%;
        display: flex;
        justify-content: space-between;
    }

    .list-item li{
        display: flex;
    }

</style>