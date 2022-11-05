<template>
  <h1>Name: {{ msg }}</h1>
  <h1>Age: {{ age }}</h1>

  <div class="">
    <h1>This Hello World Component</h1>
    <h3 id="test">test</h3>
    <ul>
      <li v-for="value in myObject" :key="value.id">
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

  props: ['msg', 'age']


}

document.getElementById("test").innerHTML = "Hello";

</script>

<style scoped>
a {
  color: #42b983;
}
</style>
