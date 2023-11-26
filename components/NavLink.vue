<script setup>
defineProps(["href", "text"]);
</script>

<template>
  <a :href="href" class="link" target="_blank" :title="href">
    {{ text }}
  </a>
</template>

<style lang="scss" scoped>
.link {
  text-decoration: none;
  font-size: 18px;
  font-weight: 500;
  display: block;
  color: #000;
  margin-bottom: 5px;
  &:hover {
    transform: scale(1.01);
    text-decoration: underline;
  }
}
</style>
