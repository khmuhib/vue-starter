<template>
  <HelloWorld msg="This is Hello Component sda" />
  <ul>
    <li v-for="value in myObject" :key="value.id">
      {{ value.title }}
    </li>
  </ul>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {

  components: { HelloWorld },
  data() {
    return {
      myObject: [
        {
          id: 1,
          title: 'How to do lists in Vue',
          author: 'Jane Doe',
          publishedAt: '2016-04-10'
        },
        {
          id: 2,
          title: 'dasdas',
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
