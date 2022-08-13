<template>
    <div>
        Todos
        <nuxt-link :to="{ name: 'todos-create'}">Create todos</nuxt-link>
        <nuxt-link :to="{ name: 'todos-todo-id' , params : { id: 5}}">Specific Todo</nuxt-link>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style>

</style>