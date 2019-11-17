<template>
  <div id="app">
    <Todos v-bind:todos="todos" />
    <img alt="Vue logo" src="./assets/logo.png" />
  </div>
</template>

<script>
import Todos from "./components/Todos";
export default {
  name: "app",
  components: {
    Todos
  },
  data() {
    return {
      todos: [
        {
          id: 1,
          title: "To Do One",
          complete: false
        },
        {
          id: 2,
          title: "To Do Two",
          complete: true
        },
        {
          id: 3,
          title: "To Do Three",
          complete: false
        }
      ]
    };
  }
};
</script>

<style>
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}
</style>
