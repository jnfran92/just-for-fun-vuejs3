<script setup>
import {ref} from "vue";

const counter = ref(0)
const increaseCount = () => {
  counter.value++
}
</script>

<template>
  <div class="main">
    <h1>This is a cat counter</h1>

    <h2 class="counter">{{ counter }}</h2>

    <button @click="increaseCount">Add a cat</button>

  </div>
</template>

<style scoped>
.main {
  text-align: center;
}
</style>