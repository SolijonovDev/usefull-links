<script setup>
useHead({
  title: "Solijonov Qodirjon",
  meta: [{ name: "description", content: "Amazing website" }],
});
</script>

<template>
  <TheHeader />
  <NuxtPage />
  <TheFooter />
</template>

<style>
* {
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
body {
  font-family: "Times New Roman", Times, serif;
  font-size: 14px;
  margin: 0;
  padding: 0;
  background-color: darkgray;
}

button {
  cursor: pointer;
}

a {
  text-decoration: none;
}
</style>
