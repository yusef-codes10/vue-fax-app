<script setup>
/*
CHALLENGE: Turn the provided HTML/CSS mockup into a Vue app that
           uses three components: Header, Main, and Footer.
           Make sure you use all the provided CSS!
*/
</script>

<template>
  <header>
    <!--
            This image has been commented out for now as it will break
            until you've learnt how to work with images!
            <img src="logo_vue_300px.png" alt="vue logo" />
            -->
    <h1>Hi, I'm <span class="highlight">Vue</span></h1>
  </header>
</template>

<style scoped>
header img {
  height: 150px;
}
header h1 {
  font-size: 2rem;
  color: #34495e;
  margin-top: 10px;
}
</style>
