<template>
  <div class="bgGroup">
    <div class="bg-1" />
  </div>
  <div class="content">
    <div class="bannerContent">
      <h1 id="title">T O D O</h1>
      <img id="toggleMode" :src="iconSun" @click="changeTheme" />
    </div>
  </div>
</template>

<script>
import bgDarkDestkop from "../assets/images/bg-desktop-dark.jpg";
import iconSun from "../assets/images/icon-sun.svg";
export default {
  data() {
    return {
      text: "Hello World",
      bg: bgDarkDestkop,
      iconSun: iconSun,
    };
  },
  methods: {
    changeTheme() {
      const html = document.getElementById("html").classList;
      if (html.contains("theme-dark")) {
        html.remove("theme-dark");
        html.add("theme-light");
      } else if (html.contains("theme-light")) {
        html.remove("theme-light");
        html.add("theme-dark");
      }
    },
  },
};
</script>

<style></style>
