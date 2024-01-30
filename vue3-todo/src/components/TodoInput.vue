<template>
    <div>
        <input type="text" v-model="todoInput" />
        <button type="button" @click="addTodo">add</button>
    </div> 
</template>

<script setup>
import { ref } from 'vue';

    // data
    const todoInput = ref('');

    // methods
    function addTodo() {
        const todo = todoInput.value;
        localStorage.setItem(todo, todo)
    }


</script>

<style lang="scss" scoped>

</style>