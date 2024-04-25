<template>
  <h1>
    {{ time }}
  </h1>
</template>

<script setup>
import { ref } from 'vue';

// Javascript here

const time = ref(new Date().toLocaleTimeString());
setInterval(() => {
  time.value = new Date().toLocaleTimeString();
}, 1000);

</script>
