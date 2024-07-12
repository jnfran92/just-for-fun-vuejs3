<script>
export default {
  name: "DogOptions",
  data() {
    return {
      counter: 0
    };
  },
  methods: {
    increaseCounter(){
      this.counter++
    }
  }
}
</script>

<template>
  <div class="main">
    <h1>This is  Dog Options counter</h1>

    <h2 class="counter">{{counter}}</h2>

    <button @click="increaseCounter">Add a Dog</button>
  </div>
</template>

<style scoped>
.main{
  text-align: center;
}
</style>