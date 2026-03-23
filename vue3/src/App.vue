<template>
  <div>
    <h1>Счётчик: {{ count }}</h1>
    <button @click="increment">Увеличить</button>
    <Child message="Привет из родительского компонента!" />
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue'
import Child from './components/Child.vue'

const count = ref(0)

const increment = () => {
  count.value++
}

onMounted(() => {
  console.log('Компонент App смонтирован!')
})
</script>