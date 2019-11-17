<template>
  <div class="todo-item" v-bind:class="{'is-complete':todo.complete}">
    <p>{{todo.title}}</p>
  </div>
</template>

<script>
export default {
  name: "TodoItem",
  props: ["todo"]
};
</script>

<style scoped>
.todo-item {
  background: #f4f4f4;
  padding: 10px;
  border-bottom: #ccc dotted;
}

.is-complete {
  text-decoration: line-through;
}

.del {
  background: #ff0000;
  color: #fff;
  border: none;
  padding: 5px 9px;
  border-radius: pointer;
  float: right;
}
</style>