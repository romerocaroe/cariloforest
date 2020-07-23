<template>
  <div id="app">
    <div id="nav">
      <img src="../media/img/logoCarilo.png" alt="logo" />
    </div>
    <div id="section">
      <div class="cuadrado1"></div>
      <div class="cuadrado2"></div>
      <div class="cuadrado3"></div>
      <div class="cuadrado4"></div>
      <div class="cuadrado5"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "mainComponent",
  props: {
    msg: String
  },
  data(){
    return{
    }
  }
};
</script>

<style scoped>
  #nav {
    padding: 10px;
  }
  .cuadrado1 {
     width: 100px; 
     height: 100px; 
     background: #ADBCC9;
  }
  .cuadrado2 {
      width: 100px; 
      height: 100px; 
      background: #377AB5;
  }
  .cuadrado3 {
      width: 100px; 
      height: 100px; 
      background: #384D5F;
  }
  .cuadrado4 {
      width: 100px; 
      height: 100px; 
      background: #1B2732;
  }
  .cuadrado5 {
     width: 100px; 
     height: 100px; 
     background: #8A8E91;
  }
</style>
