<template>
  <div class="social">
    <h3 class="social__links">
      <a href="https://github.com/alexakearns">Github</a>
    </h3>
    <h3 class="social__links">
      <a href="https://www.linkedin.com/in/alexa-kearns/">LinkedIn</a>
    </h3>
  </div>
</template>

<script>
export default {
  name: "Social",
};
</script>

<style>
.social {
  display: flex;
  justify-content: center;
}
.social__links {
  background: #7be0aa;
  border: 2px solid navy;
  border-radius: 10px;
  margin: 50px;
  padding: 20px;
}
.social__links:hover {
  background: #ff99a3;
  border-radius: 50%;
}
</style>
