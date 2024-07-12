<script>
import {ref} from "vue";
export default {
  setup(){
    const counter = ref(0)
    const increaseCount = () => {
      counter.value++
    }
    return{
      counter,
      increaseCount
    }
  }
}
</script>

<template>
  <div class="main">
    <h1>This is a Duck counter</h1>

    <h2 class="counter">{{counter}}</h2>

    <button @click="increaseCount">Add a Duck</button>

  </div>
</template>

<style scoped>
.main{
  text-align: center;
}
</style>