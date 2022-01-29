<template>
  <div>
    <app-header></app-header>
    <app-content v-bind:todos="list"></app-content>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Main from './components/Main-content.vue';

export default {
  components: {
    'app-header': Header,
    'app-footer': Footer,
    'app-content': Main
  },
  data () {
    return {
      list: [
        {name: 'Clean the room', done: false},
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

</style>
