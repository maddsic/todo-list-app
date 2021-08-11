
<template>
<!-- if completed is true in the data() defined in the app.vue component, then the .is-complete class will apply -->
    <div class="todo-item" :class="{'is-complete':todo.completed}"> 
       <p>Title: {{ todo.title }}</p> 
        <p>Completed: {{ todo.completed }}</p> 
    </div>
</template>


<script>
export default {
    // exporting our TodoItem
    name: "TodoItem",
    props: ["todo"]
}
</script>

<style scoped>

    .todo-item {
        background: #f4f4f4;
        padding: 10px;
        border-bottom: 1px #ccc dotted;
    }

    .is-complete {
        text-decoration: line-through;
    }

    .del {
        background: #ff0000;
        color: #fff;
        border: none;
        padding: 5px 9px;
        border-radius: 50%;
        cursor: pointer;
        float: right;
    }







</style>