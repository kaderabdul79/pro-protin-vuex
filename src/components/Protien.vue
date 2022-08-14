<template>
      <!-- our protien  -->
      <div id="protien" class="protien_main">
         <div class="container">
            <div class="row">
               <div class="col-md-12">
                  <div class="titlepage">
                     <h2>Our Protien</h2>
                  </div>
               </div>
            </div>
            <div class="row">
               <div class="col-md-3 col-sm-6" v-for="protien in protiens" :key="protien.id">
                  <div class="protien">
                     <router-link :to="{name: 'Details',params:{id: protien.id}}">
                        <figure><img :src="protien.img" alt="#"/></figure>
                        <h3>$ {{protien.price}}</h3>
                        <span> {{protien.name}} </span>
                     </router-link>
                     <button v-on:click="addToCart(protien.id)" class="read_more mar_top">Buy Now</button>
                  </div>
               </div>
            </div>
         </div>
      </div>
      <!-- end our protien  -->
</template>

<script>
export default {
   data(){
      return {
         protiens: [
            {id:1,name:"Variations",img:"images/pro1.png",price:500},
            {id:2,name:"Passages",img:"images/pro2.png",price:1400},
            {id:3,name:"Pedicure",img:"images/pro3.png",price:4700},
            {id:4,name:"Variations",img:"images/pro4.png",price:900},
         ]
      }
   },
   methods:{
      addToCart(protine){
         console.log(protine);
      }
   }
}
</script>

<style>

</style>