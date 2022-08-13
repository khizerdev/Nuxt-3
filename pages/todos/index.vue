<template>
    <div>
        Todos
        <nuxt-link :to="{ name: 'todos-create'}">Create todos</nuxt-link>
        <nuxt-link :to="{ name: 'todos-todo-id' , params : { id: 5}}">Specific Todo</nuxt-link>

  

        <ul>
            <li v-for="item in data">
                {{item.title}} - {{item.id}}
            </li>
        </ul>
    </div>
</template>

<script setup>

    const {data} = await useAsyncData('items' , () => $fetch('https://jsonplaceholder.typicode.com/todos') , {
        lazy:false
    });

    // const {data:todos} = useFetch('https://jsonplaceholder.typicode.com/todos')
    
</script>

<style>

</style>