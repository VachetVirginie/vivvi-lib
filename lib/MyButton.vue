<template>
  <button color="warning" @click="onClick">Click me!</button>
  <p>{{ count }}</p>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const count = ref<number>(0)

const onClick = () => {
  count.value++
  console.log(count.value)
}
</script>
