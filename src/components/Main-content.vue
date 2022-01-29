<template>
  <div id="todos">

    <ul style="list-style-type: none">
      <li v-for="todo in todos"   @click="todo.done = !todo.done"    :class="{active: todo.done}">
        <box-icon v-if="todo.done" name='checkbox-checked' color='#938e8e'></box-icon>
        <box-icon v-if="!todo.done" name='checkbox' ></box-icon>
         {{todo.name}}
      </li>
    </ul>

  </div>
</template>

<script>
export default {
  props: ['todos'],
  data () {
    return {

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
  color: black;
  text-decoration: none;
  width: max-content;
}
li.active{
  color: lightgray;
  text-decoration: line-through;
}
</style>
