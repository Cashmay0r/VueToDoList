<template>
  <comp-header> </comp-header>
  <comp-list-add></comp-list-add>
</template>

<script>
import compHeader from "./components/header.vue";
import compListAdd from "./components/listAdd.vue";

export default {
  name: "App",
  components: {
    compHeader,
    compListAdd,
  },
};
</script>

<style>
@import "./assets/styles/styles.css";
@import "./assets/styles/vars.css";

body,
html {
  background-color: var(--background-2);
}
</style>
