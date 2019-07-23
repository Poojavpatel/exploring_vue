<template>
    <div>
        <h1>This is todos component embeded in app</h1>
        <div v-bind:key="todo.id" v-for="todo in todos">
            <p>{{todo.name}}</p>
            <Todoitem v-bind:todo="todo"></Todoitem>
        </div>
    </div>
</template>

<script>
import Todoitem from './Todoitem'

export default {
    name:'Todos',
    components:{
        Todoitem,
    },
    props:["todos"],
    data(){
        return{

        }
    }
}
</script>

<style>

</style>

