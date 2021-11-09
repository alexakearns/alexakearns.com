<template>
  <div class="individual-project">
    <h2>{{ projectInfo.title }}</h2>
    <h3>{{ projectInfo.description }}</h3>
  </div>
</template>

<script>
export default {
  name: "Project",
  props: {
    name: String,
    number: String,
    projectInfo: Object,
  },
  mounted() {
    console.log(this.projectInfo);
  },
};
</script>

<style>
.individual-project {
  border: red 5px solid;
  margin: 15px;
  width: 300px;
  background: #eaeaeb;
}
</style>
