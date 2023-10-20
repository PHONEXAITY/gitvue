<template>
    <v-card>
        <div class="shoeBackground">
            <img src="blue.png" alt="" class="shoe show" color="blue" />
        </div>
        <div class="info">
          <div class="shoeName">
            <div>
              <h1 class="big">Nike Zoom KD 12</h1>
              <span class="new">new</span>
            </div>
            <h3 class="small">Men's running shoes</h3>
          </div>
          <div class="description">
            <h3 class="title">Product Info</h3>
            <p class="text">
              Lorem Ipsum is simply dummy text of the printing and typesetting
              industry. Lorem Ipsum has the industry's.
            </p>
          </div>
          </div>
          <div class="buy-price">
            <a href="#" class="buy" @click="ShoeCard"
              ><i class="fas fa-shopping-cart"></i>Add to card</a
            >
          
          </div>
    </v-card>
</template>
<script>
import ShoeCard from "@/components/shoes.vue";

export default ({
    name: 'product' ,
    components:{
       ShoeCard
    }
    ,
    data() {
        return{
            show : false
        }
    },
    methods: {
        ShoeCard () {
            this.show = true
        }
    }

});

</script>