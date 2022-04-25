<template>
 <div class="pay">  
<hr>
<br>
<a >Total</a>
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
   border: 1px solid white;
    outline-color: white;
    outline-style: solid;
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
    overflow: hidden;
    text-align: left;
    height: 10px;
    width: 500px;
    position: absolute;
 
}
@media screen and (max-width: 677px){
.pay a{
    font-size: 20px;
    margin-top:10%;
    font-family: sans-serif; 
    text-decoration-style: bold;
   
}
.pay button{
overflow: hidden;
margin-top: 10px;
margin-left: 70%;
margin-right:30%;
background: #c01444;
font-size: 16px;
padding: 15px 16px;
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
    text-align: left;
    width: 100%;
    height: 10px;
    margin-bottom: 10%; 

}

}

</style>
