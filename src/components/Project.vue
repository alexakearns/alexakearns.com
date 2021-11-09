<template>
  <div>
    <h2>{{name}} {{number}}</h2>
  </div>
</template>

<script>
export default {
  name: "Project",
  props: {
    name: String,
    number: Number,
  }
}
</script>

<style>

</style>