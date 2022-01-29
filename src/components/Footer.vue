<template>
  <div>
    <footer>
      <p>{{copyright}}</p>
    </footer>
  </div>
</template>

<script>
export default {
  data () {
    return {
      copyright: 'All rights reserved©'
    }
  }
}
</script>

<style scoped>
footer{
  background: #222;
  padding: 6px;
  border-radius: 8px;
}
p{
  color: lightgreen;
  text-align: center;
  font-size: 1.3em;
}
</style>
