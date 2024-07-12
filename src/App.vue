<script setup>
import DuckComposition from "@/components/DuckComposition.vue";
import DogOptions from "@/components/DogOptions.vue";
import CatComposition from "@/components/CatComposition.vue";
</script>

<template>
  <header>
    <CatComposition></CatComposition>
  </header>

  <main>
    <DogOptions></DogOptions>
    <DuckComposition></DuckComposition>
  </main>

  <footer>

  </footer>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
