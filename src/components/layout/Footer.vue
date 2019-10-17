<template>
    <Footer class="footer">
        <h5>Daily Todo List ~ Built with Love By <a href="https://github.com/doniyke" target="_blank"> Iyke</a></h5>
    </Footer>
</template>

<script>
export default {
    name: "footer"
}
</script>

<style scoped>
    .footer{
        background: #333;
        color: #fff;
        text-align: center;
        padding: 20px;
        margin-top: 20px;
        bottom: 0px;
        position: fixed;
        width: 100%;
    }
    a{
        text-decoration: none;
        color: goldenrod;
        font-size: 20px;
        font-weight: 900;
    }
</style>