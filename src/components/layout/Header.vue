<template>
    <header class="header">
        <h1>Daily Todo List </h1>
        <div id="nav">
            <router-link to="/">Home</router-link> |
            <router-link to="/about">About</router-link>
        </div>
    </header>
</template>

<script>
export default {
    name: "header"
}
</script>

<style scoped>
    .header{
        background: #333;
        color: #fff;
        text-align: center;
        padding: 10px;
        margin-bottom: 20px;
    }

    .header a{
        color: #fff;
        padding-right: 5px;
        text-decoration: none;
    }
    .header a:hover{
        color: goldenrod;
    }
    .router-link-active{
        color: goldenrod;
    }
    .header a:active{
        color: goldenrod;
    }
    div#nav{
        margin:20px 20px;
    }
</style>