<script setup>
useHead({
  title: "Useful websites every web developer should know",
  meta: [
    {
      name: "description",
      content: "Useful websites every web developer should know",
    },
  ],
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
