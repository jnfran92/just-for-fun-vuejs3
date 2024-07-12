<script setup>
import {reactive, ref} from "vue";

const title = ref("CatComposition");
const counter = ref(0)

const counterData = reactive({
  title: "CatComposition Two",
  count: 10,
})

const increaseCount = () => {
  counter.value++
  counterData.count++
}
</script>

<template>
  <div class="main">
    <h1>{{title}}</h1>
    <h1>This is a cat counter</h1>

    <h2 class="counter">{{ counter }}</h2>

    <button @click="increaseCount">Add a cat</button>

    <input v-model="title" type="text">


    <h1>Object Reactive</h1>
    <h1>{{counterData.title}}</h1>


    <h2 class="counter">{{ counterData.count }}</h2>

    <button @click="increaseCount">Add a cat</button>

    <input v-model="counterData.title" type="text">

  </div>
</template>

<style scoped>
.main {
  text-align: center;
}
</style>