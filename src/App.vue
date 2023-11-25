

<template>
  <div>
      <img src="../public/logoResto.jpg" class="logo vue" alt="Vue logo" />
  </div>
  <HelloWorld msg="Resto Saul" />

  <nav id="nav">
    <router-link to="/">Inicio</router-link>
    <router-link to="/categoryDetails">categoryDetails</router-link>
    <router-link to="/mealDetails">mealDetails</router-link>
  </nav>

  <router-view></router-view>


  
</template>

<script>
export default{
  name:'App',
}
</script>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #a8adffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #345345aa);
}
.category-container{
  border-radius: 10px;
  color: black;
  margin: 5% 20%;
  background-color: gray;


}
</style>