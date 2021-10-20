<template>
  <form class="contact-form" @submit.prevent="onSubmit">
    <label for="name">Name:</label>
    <input id="name" v-model="name" />
    <label for="email">Email:</label>
    <input id="email" type="email" v-model="email" />
    <label for="subject">Subject:</label>
    <input id="subject" v-model="subject" />
    <label for="message">Message:</label>
    <input id="message" v-model="message" />

    <input class="contact-form__submit" type="submit" />
  </form>
</template>

<script>
export default {
  name: "ContactForm",
  data() {
    return {
      name: "",
      email: "",
      subject: "",
      message: "",
    };
  },
  methods: {
    onSubmit() {
      let formContent = {
        name: this.name,
        email: this.email,
        subject: this.subject,
        message: this.message,
      };
      this.$emit("form-submitted", formContent);

      this.name = "";
      this.email = "";
      this.subject = "";
      this.message = "";
    },
  },
};
</script>
<style>
.contact-form {
  display: grid;
  width: 250px;
}
</style>
