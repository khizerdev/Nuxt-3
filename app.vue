<template>
  <div>
    <ul>
        <li>
          <nuxt-link :to="{ name: 'index'}">Home</nuxt-link>
          <nuxt-link :to="{ name: 'about'}">About</nuxt-link>
          <nuxt-link :to="{ name: 'todos'}">Todos</nuxt-link>
        </li>
    </ul>
    <NuxtPage/>
  </div>
</template>
