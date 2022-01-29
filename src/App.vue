<template>
  <div>
    <app-header></app-header>
    <app-content></app-content>
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

    }
  }
}
</script>

<style scoped>

</style>
