<template>
  <v-dialog max-width="600px" v-model="dialog" persistent>
    <template v-slot:activator="{ on, attrs }">
      <v-btn
        flat
        slot="activator"
        depressed
        v-bind="attrs"
        v-on="on"
        color="#0397D9"
        class="white--text mt-16"
        >Get Started</v-btn
      >
    </template>
    <v-card>
      <v-card-title>
        <h2>Contact us</h2>
      </v-card-title>
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
      <v-card-actions>
        <v-spacer></v-spacer>
        <v-btn color="blue darken-1" text @click="dialog = false">
          Close
        </v-btn>
        <v-btn color="blue darken-1" text @click="dialog = false"> Save </v-btn>
      </v-card-actions>
    </v-card>
  </v-dialog>
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
      dialog: false,
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
