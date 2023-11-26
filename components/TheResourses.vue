<script setup>
import codeEditors from "./data/code-editors.json";
import cssResourses from "./data/css-resourses.json";
import htmlResourses from "./data/html-resourses.json";
import jsResourses from "./data/js-resourses.json";
import reactJsResourses from "./data/reactjs-resourses.json";
import vueJsResourses from "./data/vuejs-resourses.json";
import nodejsResourses from "./data/nodejs-resourses.json";
import pythonResourses from "./data/python-resourses.json";
import frontendHosting from "./data/frontend-hosting.json";
import backendHosting from "./data/backend-hosting.json";
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
      <ListItem title="Angularjs" :items="nodejsResourses" />
      <ListItem title="Nodejs" :items="nodejsResourses" />
      <ListItem title="Python" :items="pythonResourses" />
      <ListItem title="Frontend Hosting Websites" :items="frontendHosting" />
      <ListItem title="Backend Server hosting" :items="backendHosting" />
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
