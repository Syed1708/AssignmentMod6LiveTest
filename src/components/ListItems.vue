<script setup>
// Question : Create a Vue component that iterates through an array of objects and displays their properties in an unordered list. The component should have the following requirements:

 

// Create a  variable named items containing an array of objects. Each object should have a name and age property.

// Use v-for to loop through the items array and display the name and age properties in separate list items.


const items =[
    {
    name: 'John', 
    age: 20 
    },
    {
    name: 'Syed', 
    age: 23
    },
    {
    name: 'Iqbal', 
    age: 22 
    },
    {
    name: 'Juwel', 
    age: 18 
    },
    {
    name: 'Ahmed', 
    age: 33 
    },

]

</script>

<template>

<div class="mx-auto container">
    <h2 text-2xl mb-10>List of Items</h2>
    <ul>
      <li class="w-80 h-10 mt-5 border" v-for="(item, index) in items" :key="index">
        Name: {{ item.name }}-- 
        Age: {{ item.age }}
      </li>
    </ul>
  </div>

</template>

<style scoped>

</style>
