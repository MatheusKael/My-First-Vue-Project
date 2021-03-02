<template>
  <div id="app">
    <Todos />
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Todos from './components/Todos.vue';

@Component({
  components: {
    Todos,
  },
})
export default class App extends Vue {

}
</script>

<style>
body{
  background-color: #f5f5f5;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
