<script setup>
import codeEditors from "./data/code-editors.json";
import cssResourses from "./data/css-resourses.json";
import htmlResourses from "./data/html-resourses.json";
import jsResourses from "./data/js-resourses.json";
import reactJsResourses from "./data/reactjs-resourses.json";
import vueJsResourses from "./data/vuejs-resourses.json";
</script>

<template>
  <div>
    <ul class="items">
      <ListItem title="Code editors" :items="codeEditors" />
      <ListItem title="Html" :items="htmlResourses" />
      <ListItem title="Css" :items="cssResourses" />
      <ListItem title="JavaScript" :items="jsResourses" />
      <ListItem title="Reactjs" :items="reactJsResourses" />
      <ListItem title="Vuejs" :items="vueJsResourses" />
    </ul>
  </div>
</template>

<style lang="scss" scoped>
.items {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  grid-gap: 20px;
}
ul,
li {
  list-style-type: none;
}
</style>
