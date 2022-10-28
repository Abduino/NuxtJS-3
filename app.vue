<script setup>
const counter = useState('counter', () => Math.round(Math.random() * 1000))
</script>
<template>
  <div>
    Counter: {{ counter }}
    <button @click="counter++">
      Increment
    </button>
    <button @click="counter--">
      Decrement
    </button>
  </div>
</template>