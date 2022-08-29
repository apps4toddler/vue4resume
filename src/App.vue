<template>
<div class="content">
  <div class="main">
    <About />
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
import About from "@/layouts/About.vue";
import Contact from "./layouts/Contact.vue";
import Skill from "./layouts/Skill.vue";
import Education from "./layouts/Education.vue";
import Publication from "./layouts/Publication.vue";
import Experience from "./layouts/Experience.vue";
import Project from "./layouts/Project.vue";
</script>

<style lang="scss">
@import "@/scss/main.scss";

.content {
  max-width: 1280px;
}

.content {
  position: relative;
  min-width:320px;
  margin: var(--space-6) auto;
  padding: var(--space-6) 0;
  box-shadow:
    0 8px 16px rgb(110 120 130 / 12%),
    0 -8px 16px rgb(110 120 130 / 12%);
  background: var(--light);
}

.main {
  display: flex;
  flex-direction:column;
  height: calc(100vh - calc((var(--space-6) * 4)));
  overflow-x: hidden;
  overflow-y: scroll;
}

</style>
