<template>
  <h1>{{my_name}}</h1>
  <h3>{{job_title}}</h3>
</template>

<script>
export default {
  name: "Intro",
  props: {
    my_name: String,
    job_title: String,
  },
}
</script>

<style>

</style>