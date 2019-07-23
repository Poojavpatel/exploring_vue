<template>
    <div v-bind:class="{'iscomplete':todo.completed}">
        <p>
        {{todo}}
        </p>
    </div>
</template>

<script>
export default {
    name:"Todoitem",
    props:["todo"],
}
</script>

<style scoped>
    .iscomplete{
        text-decoration: line-through;
    }
</style>
