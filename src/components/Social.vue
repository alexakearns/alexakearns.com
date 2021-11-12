<template>
  <div class="social">
    <h3 class="social__links">
      <a href="https://github.com/alexakearns" target="_blank">
        <img src="@/assets/images/github.png" alt="linkedin" class="social__links-icons">
      </a>
    </h3>
    <h3 class="social__links">
      <a href="https://www.linkedin.com/in/alexa-kearns/" target="_blank">
        <img src="@/assets/images/linkedin.png" alt="linkedin" class="social__links-icons">
      </a>
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
  border-radius: 10px;
  margin: 50px;
  padding: 20px;
}
.social__links-icons {
  height: 70px;
}
.social__links:hover {
  transform: scale(1.1);
}
</style>
