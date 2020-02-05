<template>
  <div id="app">
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>
import Todos from './components/Todos.vue'
export default {
  name: 'app',
  components: {
    Todos
  },
  data(){
    return {
      todos: [
        {
          id:1, 
          title: "ToDo one",
          completed:false
        },
        {
          id:2, 
          title: "ToDo Two",
          completed:true
        },
        {
          id:3, 
          title: "ToDo three",
          completed:false
        }
      ]
    }
  }
}
</script>

<style>
</style>
