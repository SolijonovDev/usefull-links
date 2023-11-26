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
    </div>
  </li>
</template>

<style lang="scss" scoped>
.item{
  background-color: rgba(60, 255, 20,.9);
  padding:15px;
  border-radius: 10px;
}
.title {
  font-size: 26px;
  font-weight: 600;
  margin-bottom: 12px;
}
</style>
