<template>
  
    <div class="">
      <h1>User Component</h1>
      <ul>
        <li v-for="value in data" :key="value.id">
          {{ value.title }}
        </li>
      </ul>
    </div>
  
  
  </template>
  
  <script>
  export default {
    data() {
      return {
      }
    },
  
    props: ['msg', 'age', 'data']
  
  
  }
  
  </script>
  
  <style scoped>
  a {
    color: #42b983;
  }
  </style>
  