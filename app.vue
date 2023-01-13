<script setup>
const counter = ref(0);

const add = () => {
  counter.value = counter.value + 1;
};
const subtract = () => {
  counter.value = counter.value - 1;
};
</script>

<template>
  <div class="main">
    <h1>Counter application in NUXT JS</h1>
    <div class="counter">
      <button @click="subtract">-</button>
      <div>{{ counter }}</div>
      <button @click="add">+</button>
    </div>
  </div>
</template>

<style scoped>
.main {
  background-color: rgb(206, 206, 233);
  height: 100vh;
  width: 100%;
  margin: 0;
  padding: 0;
}
h1 {
  margin: 0;
  padding: 0;
}
.counter {
  display: flex;
  align-items: center;
  justify-content: center;
}
button {
  padding: 10px;
  margin: 10px;
}
h1 {
  text-align: center;
}
</style>
