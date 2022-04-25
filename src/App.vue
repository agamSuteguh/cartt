<template>
  <div id="app">
    
    <heade/>
    <CartMain/>
    <pay/>

  </div>
</template>

<script>
import heade from './components/head.vue'
import CartMain from './components/cart.vue'
import pay from './components/payment.vue'
export default {
  name: 'App',
  components: {
    heade,
    CartMain,
    pay
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
margin-left: 30%;
margin-right: 30%;
}

@media screen and (max-width: 677px){
  #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
margin-left: 20%;
margin-right: 30%;
}

}


</style>
