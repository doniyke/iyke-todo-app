<template>
  <div id="app">
      <AddTodo v-on:add-todo="addTodo"/>
      <Todos v-bind:todos = "todos" v-on:del-todo="deleteTodo"/>
  </div>
</template>

<script>

import  AddTodo from '../components/AddTodo';
import Todos from '../components/Todos';


export default {
  name: 'home',
  components: {
    AddTodo,
    Todos
  },
  data(){
    return {
     todos : []
    }
  },
  methods:{
    deleteTodo(id){
      this.todos = this.todos.filter(todo => todo.id !== id);
    },
    addTodo(newTodo){
      this.todos = [...this.todos, newTodo];
    }
  },
  created(){

  }
}
</script>

<style>
  *{
    box-sizing: border-box;
    margin : 0;
    padding :0;
  }

  body{
    font-family:Arial, Halvetica, sens-serif;
    line-height:1.4;
  }

  .btn {
    display: inline-block;
    border: none;
    background: #555;
    color: #fff;
    padding: 7px 20px;
    cursor: pointer;
  }

  .btn:hover{
    background: #666;
  }
</style>
