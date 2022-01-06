<template>
  <div id="app">
    <TodoList v-bind:todos="todos"/>
  </div>
</template>

<script>
import TodoList from './components/TodoList'

export default {
  name: 'App',
  components: {
    TodoList
  },
  data () {
    return {
      todos: [{
        name: 'Ankit',
        email: 'abc@gmail.com',
        desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
        status: 'To Do'
      }, {
        name: 'Dheeraj',
        email: 'def@gmail.com',
        desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
        status: 'Done'
      }, {
        name: 'Abhishek',
        email: 'pqr@gmail.com',
        desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
        status: 'Doing'
      }, {
        name: 'Juzer',
        email: 'xyz@gmail.com',
        desc: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit',
        status: 'Done'
      }]
    }
  }
}
</script>
