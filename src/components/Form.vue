<template>
  <v-card>
    <v-form class="px-3" id="contact_form">
      <v-text-field label="Name" v-model="name" class="name"></v-text-field>
      <v-text-field
        label="Last Name"
        v-model="last_name"
        class="last_name"
      ></v-text-field>
      <v-textarea label="Message" v-model="message"></v-textarea>
      <v-btn flat class="success mx-0 mt-3" @click="submit">Send</v-btn>
    </v-form>
  </v-card>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Form",
  data() {
    return {
      name: "",
      last_name: "",
      message: "",
    };
  },
  methods: {
    submit() {
      console.log(this.title, this.content);
    },
  },
};
</script>

<style scoped>
#contact_form {
  margin: 50px 0 0 0;
}
</style>
