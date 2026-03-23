<template>
  <h1>Hello {{ msg }}</h1>
  <input v-model="msg" />
  <p>Счётчик: {{ count }}</p>
  <button @click="count++">Увеличить</button>
</template>

<script setup>
import { ref } from 'vue'

const msg = ref('World')
const count = ref(0)
</script>