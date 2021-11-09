<template>
  <div class="all-projects">
    <h1 class="all-projects__heading">My Projects</h1>
    <div class="all-projects__container">
      <!-- <Project name="First" number="1" />
      <Project name="Second" number="2" />
      <Project name="Third" number="3" /> -->
      <div v-for="project in projectsData" v-bind:key="project.title">
        <Project :projectInfo="project" />
      </div>
    </div>
  </div>
</template>

<script>
import Project from "@/components/Project.vue";
import json from "../assets/ProjectDetails.json";

export default {
  name: "AllProjects",
  components: {
    Project,
  },
  data() {
    return {
      projectsData: json,
    };
  },
  mounted() {
    console.log(this.projectsData);
    console.log(this.projectsData[0].title);
  },
};
</script>

<style>
/* .projects {
  border: 5px solid purple;
  display: flex;
  justify-content: space-evenly;
} */

/* .all-projects {
  display: flex;
} */

.all-projects__heading {
  background: black;
  color: white;
  margin: 0 300px;
}

.all-projects__container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-evenly;
  margin-top: 5vh;
}
</style>
