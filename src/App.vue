<template>
  <main>
    <div>
      <h4>The current count is .... </h4>
      <h1>{{ count }}</h1>
      <button @click="count++">+</button>
      <button @click="count--">-</button>
    </div>
  </main>
</template>

<script>
  export default {
    data() {
      return {
        count: 0
      }
    }
  }
</script>

<style>
  main {
    background-color: antiquewhite;
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