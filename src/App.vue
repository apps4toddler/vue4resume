<template>
<div class="content">
  <div class="main">
    <Introduction />
    <Contact />
    <Skill />
    <Education />
    <Publication />
    <Experience />
    <Project />
  </div>
  <Switches />
</div>
</template>

<script setup lang="ts">
import Switches from "@/layouts/Switches.vue";
import Introduction from "@/layouts/Introduction.vue";
import Contact from "./layouts/Contact.vue";
import Skill from "./layouts/Skill.vue";
import Education from "./layouts/Education.vue";
import Publication from "./layouts/Publication.vue";
import Experience from "./layouts/Experience.vue";
import Project from "./layouts/Project.vue";
</script>

<style lang="scss">

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
