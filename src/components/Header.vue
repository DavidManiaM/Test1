<template>
  <div>
    <header>
      <h1>{{title}}</h1>
      <p>{{list}}</p>
    </header>
  </div>
</template>

<script>
export default {
  data () {
    return {
      title: 'Official todo list😎!'
    }
  }
}
</script>

<style scoped>
header{
  background: lightgreen;
  padding: 10px;
  border-radius: 8px;
}

h1 {
  color: #222;
  text-align: center;
}
</style>
