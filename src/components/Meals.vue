<template>
<div @click="openCategoryList" class="category-container">
      <img :src="meal.strMealThumb" alt="">
      <h3>{{ meal.strMeal }}</h3>
      <p>Categoria: {{ meal.strCategory }} | Origen:{{ meal.strArea }} </p>
  </div>
  </template>
  
  <script>
  export default{
    props:["category"]
  }
  </script>