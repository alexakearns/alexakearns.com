<template>
  <h1>Get in touch.</h1>
  <ContactForm />
  <Social />
</template>

<script>
import ContactForm from "@/components/ContactForm.vue";
import Social from "@/components/Social.vue";

export default {
  name: "Contact",
  components: {
    ContactForm,
    Social,
  },
};
</script>

<style></style>
