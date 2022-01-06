<template>
  <div class="container">
    <div class="row">
      <Todo v-for="todo in todos" :key="todo.email" v-bind:todo="todo"/>
    </div>
  </div>
</template>

<script>
import Todo from './Todo'
export default {
  name: 'TodoList',
  props: ['todos'],
  components: {
    Todo
  }
}
</script>
