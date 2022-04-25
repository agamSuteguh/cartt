<template>
  <div class="buton">
    <p v-for="item in items" :key="item.nama">
         {{item.nama}}
    </p>
    <p v-for="item in items" :key="item.harga">
         {{item.harga}}
    </p>

  <button v-for="item in items" :key="item.wish" @click="item.wish--;" :disabled="item.wish == 0"> - </button>
  <a v-for="item in items" :key="item.wish" >{{( item.wish )}}</a>
  <button v-for="item in items" :key="item.wish+item.qty"  @click="item.wish++;" :disabled="item.wish == item.qty">+ </button>


</div>





</template>

<script>
import item from './products/products.json'

export default {
  name: 'CartMain',
 data() {
   return{
   items: item
}
    }
  }




</script>
<style scoped>
.button {
  overflow: hidden;

}
.buton button{
 padding: 10px 10px;
  font-size: 15px;
  text-align: center;
  background-color: #f8f9fabc;
  border: none;
 

  
}
.buton button:hover {
  background-color: #ececec;

  }

.buton a{
  padding: 10px 100px;
  background-color: #ececec;
   border: 1px solid #ccd4dc  ;
  border-radius: 10px;
}
.buton container{
  padding: 101px ;
background-color: gray;
}
@media screen and (max-width: 677px){
  .button {
  overflow: hidden;

}
.buton button{
 padding: 3px 5px;
  font-size: 7px;
  text-align: center;
  background-color: #f8f9fabc;
  border: none;
  
 

  
}
.buton button:hover {
  background-color: #ececec;

  }

.buton a{
  padding: 4px 40px;
  background-color: #ececec;
   border: 1px solid #ccd4dc  ;
  border-radius: 10px;
  font-size: 7px;
}
.buton container{
  padding: 11px ;
background-color: gray;
}
.buton p{
  font-size: 7px;
}
}

</style>
