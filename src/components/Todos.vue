
<template>
    <div>
        <div v-for="todo in todos" :key="todo.id">
            <TodoItem :todo="todo" />
        </div>
    </div>
</template>

<script>

import TodoItem from './TodoItem.vue'

export default {
    name: "Todos",

    components: {
        TodoItem 
    },
    props: [ "todos" ]
}
</script>

<style scoped>
h1{
    color: black;
}
</style>