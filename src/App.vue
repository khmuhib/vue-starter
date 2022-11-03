<template>
  <HelloWorld msg="Kh Muhib" age="23"/>
  <User v-bind:data="myObject"/>

  <ul>
    <h1>This is App.vue</h1>
    <li v-for="value in myObject" :key="value.id">
      {{ value.title }}
    </li>
  </ul>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import User from './components/User.vue'

export default {

  components: { HelloWorld, User },
  data() {
    return {
      myObject: [
        {
          id: 1,
          title: 'aaa',
          author: 'Jane Doe',
          publishedAt: '2016-04-10'
        },
        {
          id: 2,
          title: 'bbb',
          author: 'dsadas',
          publishedAt: 'dsadsad'
        },
        {
          id: 3,
          title: 'ccc',
          author: 'dsadas',
          publishedAt: 'dsadsad'
        },
        {
          id: 4,
          title: 'ddd',
          author: 'dsadas',
          publishedAt: 'dsadsad'
        },
        {
          id: 5,
          title: 'eee',
          author: 'dsadas',
          publishedAt: 'dsadsad'
        },
        {
          id: 6,
          title: 'fff',
          author: 'dsadas',
          publishedAt: 'dsadsad'
        },
        {
          id: 6,
          title: 'fff',
          author: 'dsadas',
          publishedAt: 'dsadsad'
        },
        {
          id: 6,
          title: 'fff',
          author: 'dsadas',
          publishedAt: 'dsadsad'
        },
      ]
    }
  }

}


</script>

<style>

</style>
