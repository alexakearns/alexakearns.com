<template>
  <div>
    <div class="intro">
      <h1 class="intro__name">{{ my_name }}</h1>
      <div class="intro__job">
        <h3>{{ job_title }}</h3>
        <a :href="company_url" target="_blank">
          <img :src="require(`@/assets/images/${company_icon}`)" alt="{icon_alt}" class="intro__icon">
        </a>
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
  name: "Intro",
  props: {
    my_name: String,
    job_title: String,
    company_url: String,
    company_icon: String,
    icon_alt: String,
  },
};
</script>

<style>


.intro__name {
  /* padding: 15px; */
  font-size: 45px;
}

.intro__job {
  display: flex;
  justify-content: center;
}

.intro__icon {
  height: 70px;
  margin-left: 10px;
}
</style>
