<template>
  <main>
    <div>
      <h4>
      The current count is..
    </h4>
    <h1>{{ count }}</h1>
    <button @click="count++">+</button>
    <button @click="count--">-</button>
    </div>    
  </main>
</template>

<script setup>
  import {ref} from 'vue';
  
  const count = ref(0);
</script>

<style scoped>
main {
  background-color: aliceblue;
  height: 100vh;
  width: 100vw;
  display: flex;
  align-items: center;
  justify-content: center;
}
div {
  color: black;
}
</style>