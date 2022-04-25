<template>

 <div class="pay">  
<hr>
<br>
<a >TOTAL</a>
<br>
  <a v-for="item in items" :key="item.wish+item.harga">Rp.{{(  item.wish*item.harga )}}</a> <button v-on:click="res">Bayar</button> 
  
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

.pay a{
    font-size: 18px;

}
.pay button{
margin-left: 350px;
background: #c01444;
border: none;
padding: 10px 20px;
color: white;
border-radius: 10px;
position: absolute;

}
.pay button:active{
  outline-style: solid;
  outline-color: rgb(209, 242, 255);


}
hr {
  border: none;
    background-color: #f0ecec;
    overflow: visible;
    text-align: left;
    height: 20px;
    width: 500px;
    
}
@media screen and (max-width: 677px){
  

.pay a{
    font-size: 7px;
}
.pay button{
  margin-top: 10px;
margin-left: 125px;
background: #c01444;
font-size: 5px;
padding: 4px 5px;
color: white;
border-radius: 5px;
position: absolute;

}
.pay button:active{
  outline-style: solid;
  outline-color: rgb(209, 242, 255);


}
hr {
  border: none;
    background-color: #f0ecec;
    overflow: hidden;
    text-align: left;
     width: 200px;
	height: 10px; 
    position: absolute;
}

}

</style>
