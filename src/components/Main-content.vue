<template>
  <div id="todos">

    <ul style="list-style-type: none">
      <li v-for="todo in todos"    @click="todo.done = !todo.done;"     :class="{active: todo.done}">
        <box-icon v-if="!todo.done" name='checkbox-checked' color='#938e8e' ></box-icon>
        <box-icon v-if="todo.done" name='checkbox' ></box-icon>
         {{todo.name}}
      </li>
    </ul>

  </div>
</template>

<script>
export default {
  data () {
    return {
      todos: [
        {name: 'Clean the room', done: true},
        {name: 'Wash the dishes', done: false},
        {name: 'Go for a walk', done: false},
        {name: 'Go to school', done: false},
        {name: 'Do homework', done: false},
        {name: 'Relax', done: false}
      ]
    }
  }
}
</script>

<style scoped>
*{
  user-select: none;
  font-size: 1.2em;
}
li:hover{
  cursor: pointer;
}
li{
  color: lightgray;
  text-decoration: line-through;
  width: max-content;
}
li.active{
  color: black;
  text-decoration: none;
}
</style>
