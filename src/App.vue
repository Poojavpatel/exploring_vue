<template>
  <div id="app">
    <h1>{{msg}}</h1>
    <Todos v-bind:todos="todos"></Todos>
  </div>
</template>

<script>
import Todos from './components/Todos'

export default {
  name: 'app',
  components: {
    Todos,
  },
  data(){
    return{
      msg:"This is app component",
      todos:[
        {name:"Task1", id:1, completed:false},
        {name:"Task2", id:2, completed:true},
        {name:"Task3", id:3, completed:false},
      ],
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  margin-top: 60px;
  font-size: 16px;
  text-align: center;
}
</style>
