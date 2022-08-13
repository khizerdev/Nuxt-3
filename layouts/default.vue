<template>
    <div>
        <ul>
            <li>
            <nuxt-link :to="{ name: 'index'}">Home</nuxt-link>
            <nuxt-link :to="{ name: 'about'}">About</nuxt-link>
            <nuxt-link :to="{ name: 'todos'}">Todos</nuxt-link>
            </li>
        </ul>

        <slot/>

        <div>
            Footer
        </div>

    </div>
</template>

<script>
    export default {
        
    }
</script>

<style>

</style>