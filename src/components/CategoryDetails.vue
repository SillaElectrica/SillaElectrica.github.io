<template>
    <p>Lista de recetas por categoria</p>
    <h3>{{ category_title }}</h3>
    <Meals v-for="meal in meals" v-bind:key="meal.idMeal" v-bind:meal="meal"/>
</template>

<script>
import Meals from './Meals.vue'
import axios from 'axios'

export default{
    name: "CategoryDetails",
    components:{
        Meals,
    },

    data(){
        return{
            category_title: "Nombre de cat",
            meals: [],
            page: 1, 
            pages: 1
        }
    },
    mounted(){
            console.log(this.$route.params)
        }
}


</script>