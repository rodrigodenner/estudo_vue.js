<template>
  <div>
    <h2>Lista de Tarefas</h2>
    <img src="https://placehold.co/400" alt="Foto aleatoria">
    <ul>
      <li v-for="todo in todos" v-bind:key=todo.id>
        {{ todo.title }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      todos: [
        {
          "userId": 1,
          "id": 1,
          "title": "delectus aut autem",
          "completed": false
        },
        {
          "userId": 1,
          "id": 2,
          "title": "quis ut nam facilis et officia qui",
          "completed": false
        },
        {
          "userId": 1,
          "id": 3,
          "title": "fugiat veniam minus",
          "completed": false
        },
        {
          "userId": 1,
          "id": 4,
          "title": "et porro tempora",
          "completed": true
        }
      ]
    }
  }
}
</script>
