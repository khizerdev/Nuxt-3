<template>
    <div>
        Todo
        <div>
            {{todo}}
        </div>
    </div>
</template>

<script setup>

    const route = useRoute()

    const {data:todo} = await useFetch(`https://jsonplaceholder.typicode.com/todos/${route.params.id}` , {
        pick:['id','title']
    })

</script>