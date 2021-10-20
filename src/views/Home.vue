<template>
  <div class="home">
    <Intro my_name="Alexa Kearns" job_title="Frontend Engineer" />
  </div>
</template>

<script>
import Intro from "@/components/Intro.vue";

export default {
  name: "Home",
  components: {
    Intro,
  },
};
</script>
