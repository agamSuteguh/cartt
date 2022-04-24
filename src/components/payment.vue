<template>
 <div class="pay">  
<p>.</p>
<a >TOTAL</a>
<br>
  <a v-for="item in items" :key="item.wish+item.harga">Rp.{{(  item.wish*item.harga )}}</a>
   <button v-on:click="res">Bayar</button>

</div>


</template>

<script>
import item from './products/products.json'

export default {
  name: 'payMent',
  data(){
    return{
      items:item
  }
 },
 methods: {
    res: function () {
      alert('transaksi anda berhasil di proses')
    
    }}
}
   
      

      

  

    





</script>
<style scoped>
.pay p {
    color: #f0ecec ;
    background-color:#f0ecec ;
    margin-right: 8.5%;
}
.pay a{
    font-size: 18px;
}
.pay button{
margin-left: 325px;
background: #c01444;
border: none;
padding: 10px 20px;
color: white;
border-radius: 10px;

}
.pay button:active{
  outline-style: solid;
  outline-color: rgb(209, 242, 255);


}

</style>
