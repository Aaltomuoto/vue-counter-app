<script setup>
  import {ref} from "vue";

  const count = ref(10);

  const addToCount = () => {
    count.value++;
  }
  const subtractFromCount = () => {
    count.value--;
  }
</script>

<template>
  <main>
    <div>
      <h4>The current count is</h4>
      <h1>{{ count }}</h1>
      <button @click="subtractFromCount">-</button>
      <button @click="addToCount">+</button>
    </div>
  </main>
</template>

<style scoped>
main {
  background-color: var(--color-background);
  height: 100vh;
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: center;
}
div {
  text-align: center;
}

</style>