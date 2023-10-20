<template>
<v-app-bar app color="secondary" height="102" class="py-36">

      <v-app-bar-nav-icon variant="text" @click.stop="drawer = !drawer"></v-app-bar-nav-icon>

        <v-toolbar-title>LailaoLab</v-toolbar-title>

        <v-spacer></v-spacer>
        <div class="mr-12">
    <span><a href="" class="text-decoration-none mr-10 text-black shadow-lg hover:bg-transparent" id="homepage" >Home</a></span>
    <span><a href="" class=" text-decoration-none mr-10">Blog</a></span>
    <span><a href="" class="text-decoration-none mr-10">AboutUs</a></span>
    <span><a href="" class="text-decoration-none text-black">Contact</a></span>
  </div>
      </v-app-bar>

      <v-navigation-drawer
        v-model="drawer"
        location="left"
        temporary
      >
        <v-list
          :items="items"
        ></v-list>
      </v-navigation-drawer>
  
  <v-spacer></v-spacer>

  <!---->
  
    <v-container>
          <v-card>
         <Product_Card />
          </v-card>   
    </v-container>



  


</template>

<script>
import { defineComponent } from 'vue';

import Product_Card from "@/components/product.vue";
// Components


export default defineComponent({
  name: 'HomeView',
  
 
  components: {
   Product_Card
   
  },

});
</script>
<style type="text/tailwindcss">
@layer utilities {
  .content-auto {
    content-visibility: auto;
  }
}




</style>