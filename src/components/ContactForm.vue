<template>
  <div class="contact">
    <div class="contact__container">
      <form class="contact-form" @submit.prevent="onSubmit">
        <div class="contact-form__2-up">
          <input id="name" v-model="name" placeholder="Name" />
          <input id="email" type="email" v-model="email" placeholder="Email" />
        </div>
        <input id="subject" v-model="subject" placeholder="Subject" />
        <input id="message" v-model="message" placeholder="Message" />

        <input class="contact-form__submit" type="submit" />
      </form>
    </div>
  </div>
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
.contact__container {
  /* position: relative; */
  display: flex;
  justify-content: center;
}

.contact-form {
  display: grid;
  width: 250px;
  /* position: absolute; */
  /* left: 50%;
  top: 50%; */
}

.contact-form__2-up {
  display: flex;
  margin-bottom: 5px;
}

.contact-form__2-up #name {
  margin-right: 2.5px;
}

.contact-form__2-up #email {
  margin-left: 2.5px;
}

.contact-form__2-up #message {
  height: 50px;
}

.contact-form__submit {
  margin: 15px;
}
</style>
