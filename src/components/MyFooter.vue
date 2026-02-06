<script setup>
import { ref } from 'vue'

const link = ref('https://vuejs.org/')
</script>

<template>
  <footer>
    <p>Learn more about me at <a target="_blank" v-bind:href="link">vuejs.org</a></p>
  </footer>
</template>

<style scoped>
footer {
  margin-top: 35px;
  font-size: 0.8rem;
}

a {
  color: #40b883;
}
</style>
