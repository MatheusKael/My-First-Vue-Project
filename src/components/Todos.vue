<template>
  <div class="todoapp">
    <h1>To Do's</h1>
    <input type="text" class="new-todo"
      autofocus
      autocomplete='off'
      v-model="newTodo"

     />
  </div>
</template>

<script lang="ts">

import { Component, Prop, Vue } from 'vue-property-decorator';

@Component
export default class Todos extends Vue {

  // @Prop() private msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.new-todo {
  width: 500px;
  height: 40px;
  font-size: 20px;
  padding: 16px 16px 16px 60px;
  background-color: rgba(248, 248, 248, 0.003);
  border-radius: 10px;
  border: none;
  box-shadow: 1px -2px 20px rgba(0, 0, 0, 0.268);
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.new-todo:focus {
  outline: none;
}
.edit {
  outline: none;
}
h1 {
  font-size: 60px;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
