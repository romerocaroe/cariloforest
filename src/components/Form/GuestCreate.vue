<template>
    <v-row>
      <v-col cols="12">
        <ul>
          <li v-for="(guest,index) in guests" :key="index">{{guests}}</li>
        </ul>
        <guestForm v-model="form"
                  ref="form"></guestForm>
      </v-col>
    </v-row> 
    <!-- 
    <div id="section">
      <div class="cuadrado1"></div>
      <div class="cuadrado2"></div>
      <div class="cuadrado3"></div>
      <div class="cuadrado4"></div>
      <div class="cuadrado5"></div>
    </div> -->
</template>

<script>
  import GuestForm from './GuestForm';

   export default {
    name: "GuestNew",
    components: {
        GuestForm
    },
    data(){
      return {
        guests: ["uno","dos","tres"]
      }
    }
  }
</script>

<style scoped>
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
