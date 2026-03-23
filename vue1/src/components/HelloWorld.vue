<template>
  <div>
    <h1>Привет, Дима!</h1>
    <p>Это моё первое приложение на Vue.js</p>
  </div>
  <div>
    <h1>Счётчик: {{ count }}</h1>
    <button @click="increment">Увеличить</button>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)

const increment = () => {
  count.value++
}
</script>