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
import freeFakeApis from "./data/free-fake-apis.json";
import codingPractise from "./data/coding-practise.json";
import codingStyle from "./data/coding-style.json";
import codeRepositories from "./data/code-repositories.json";
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
      <ListItem title="Free fake apis" :items="freeFakeApis" />
      <ListItem title="Frontend Hosting Websites" :items="frontendHosting" />
      <ListItem title="Backend Server hosting" :items="backendHosting" />
      <ListItem title="Coding practise for beginners" :items="codingPractise" />
      <ListItem title="Coding style" :items="codingStyle" />
      <ListItem title="Code repositories" :items="codeRepositories" />
    </ul>
  </div>
</template>

<style lang="scss" scoped>
.items {
  display: grid;
  grid-template-columns: repeat(1, 1fr);
  grid-gap: 10px;

  @media (min-width: 500px) {
    grid-template-columns: repeat(2, 1fr);
    grid-gap: 15px;
  }

  @media (min-width: 720px) {
    grid-template-columns: repeat(3, 1fr);
  }

  @media (min-width: 950px) {
    grid-template-columns: repeat(4, 1fr);
    grid-gap: 20px;
  }

  @media (min-width: 1200px) {
    grid-template-columns: repeat(5, 1fr);
  }
}
ul,
li {
  list-style-type: none;
}
</style>
