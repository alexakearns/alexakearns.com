<template>
  <div class="projects">
    <h1>Projects</h1>
    <AllProjects />
    <Home />
  </div>
</template>

<script>
import AllProjects from "@/components/AllProjects.vue";

export default {
  name: "Projects",
  components: {
    AllProjects,
  },
};
</script>

<style></style>