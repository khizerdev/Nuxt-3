<template>
    <div>
        Todo
        <div>
            {{todo.title}}
        </div>
    </div>
</template>

<script setup>

    const route = useRoute()

    const {data:todo} = await useFetch(`https://jsonplaceholder.typicode.com/todos/${route.params.id}` , {
        pick:['id','title']
    })

    useMeta({
        title: todo.value.title
    })

</script>