<script setup>
import HelloWorld from './components/HelloWorld.vue'
import { Button, Input } from '@dm/components'
import { getUser } from '@dm/api'

getUser().then(res => {
  console.log('res', res)
})
// console.log('getUser', getUser)
</script>

<template>
  <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <h1>这是一段自定义的时候的匡扶汉室看到</h1>
  <HelloWorld msg="Vite + Vue" />
  <Button />
  <Input />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
