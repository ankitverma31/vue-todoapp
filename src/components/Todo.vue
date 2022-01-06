<template>
  <div class="col-sm-6">
    <div class="card my-2">
      <div class="card-body">
        <h5 class="card-title">{{ todo.name }} <span class="badge rounded-pill float-end" v-bind:class="{ 'bg-success': todo.status == 'Done', 'bg-primary': todo.status == 'Doing', 'bg-warning': todo.status == 'To Do' }">{{ todo.status }}</span></h5>
        <hr>
        <p class="card-text">{{ todo.email }}</p>
        <p class="card-text">{{ todo.desc }}</p>
        <div class="btn-group" role="group">
          <button type="button" class="btn btn-primary">Edit</button>
          <button type="button" class="btn btn-danger">Delete</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Todo',
  props: ['todo']
}
</script>
