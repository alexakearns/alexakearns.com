<template>
  <div class="home">
    <Intro my_name="Alexa Kearns" job_title="Frontend Engineer at Potato" company_icon="potato.png" company_url="https://p.ota.to/" alt="Potato logo"/>
    <Social />
  </div>
</template>

<script>
import Intro from "@/components/Intro.vue";
import Social from "@/components/Social.vue";

export default {
  name: "Home",
  components: {
    Intro,
    Social,
  },
};
</script>

<style>
.home {
  align-content: center;
  background: #000;
  bottom: 0;
  height: 80vh;
  left: 0;
  margin: 5%;
  opacity: 0.8;
  right: 0;
  padding: 20px;
  position: absolute;
  text-align: center;
  top: 0;
  /* mix-blend-mode: screen; */
  /* z-index: 1; */
}
</style>
