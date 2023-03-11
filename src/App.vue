<script setup>
  import { ref } from "vue"
  const count = ref(0);
  const addToCount = () => { 
  count.value = count.value+1
  }
  const substractToCount = () => {
    count.value = count.value-1
  }

</script>

<template>
  <main>
    <div>
      <h4>The current count is : </h4>
      <h1>{{ count }}</h1>
      <button @click="addToCount">+</button>
      <button @click="substractToCount">-</button>
    </div>
  </main>
</template>

<style scoped>
  main {
    background-color: hsl(183, 65%, 84%);
    height: 100vh;
    width: 100vw;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  div {
    text-align: center;
  }

  button {
    margin: 4px;
    padding: 4px;
  }

</style>