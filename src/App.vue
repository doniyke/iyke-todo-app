<template>
  <div id="app">
    <Header />
    <router-view/>
    <Footer />
  </div>
</template>

<script>
import Header from "./components/layout/Header";
import Footer from "./components/layout/Footer";
export default {
  name :"app",
  components:{
    Header,
    Footer
  }
}
</script>


<style>
  *{
    box-sizing: border-box;
    margin : 0;
    padding :0;
  }

  body{
    font-family:Arial, Halvetica, sens-serif;
    line-height:1.4;
    
  }

  .btn {
    display: inline-block;
    border: none;
    background: #555;
    color:goldenrod;
    padding: 7px 20px;
    cursor: pointer;
  }

  .btn:hover{
    background: #666;
  }
</style>
