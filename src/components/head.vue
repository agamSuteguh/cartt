<template>

<div class="topnav">
 <b> <a href="#home">Product List </a></b>
</div>
</template>

<script>

export default {
  name: 'HeadeR',

}




</script>


<style scoped>


.topnav {
  background-color: #c01444;
  overflow: hidden;
  width: 500px;
	height: 30px; 
  text-align: center;
  padding-top: 20px;
}

.topnav a {
  color: #f2f2f2;
  text-decoration: none;


}


@media screen and (max-width: 677px) {

.topnav {
  background-color: #c01444;
  overflow: hidden;
  width: 200px;
	height: 17px; 
  text-align: center;
  padding-top: 3px;
}

.topnav a {
  color: #f2f2f2;
 text-align: center;
  font-size: 7px;
  margin-bottom: 50%;
}
}
</style>
