<script setup>
defineProps(["title", "items"]);
</script>

<template>
  <li class="item">
    <h2 class="title">{{ title }}</h2>
    <div>
      <template v-for="item in items">
        <NavLink :href="item.href" :text="item.text" />
      </template>
      <slot />
      <!-- <a href="https://www.w3schools.com/html/default.asp">w3schools.com (en)</a> -->
    </div>
  </li>
</template>

<style lang="scss" scoped>
.title {
  font-size: 26px;
  font-weight: 600;
  margin-bottom: 12px;
}
</style>
