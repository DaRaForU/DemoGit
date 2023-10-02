<script setup>
  import {ref} from 'vue';
  const count = ref(0);

  const addToCount = () => {
    count.value += 1;
  };

  const subStractToCount = () => {
    count.value -= 1;
  };

  console.log(typeof count)
</script>

<template>
  <main>
    <div>
      <h1>The Current...</h1>
      <h1>{{ count }}</h1>
      <button @click="addToCount()">+</button>
      <button @click="subStractToCount()">-</button>
    </div>
  </main>
</template>

<style scoped>
  main{
    width: 100wh;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    color: red;
  }
  div{
    align-items: center;
  }
</style>