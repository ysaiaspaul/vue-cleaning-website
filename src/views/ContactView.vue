<template>
  <div class="contact">
    <v-container app>
      <v-layout column>
        <v-flex class="display-2 text-center my-5">Contact Us</v-flex>
        <p class="display-1 text-center my-5">Tell us what you need.</p>
      </v-layout>
      <v-row class="text-center my-5">
        <v-col md="4">
          <v-icon size="150" class="hidden-md-and-down"
            >mdi-map-marker-radius</v-icon
          >
        </v-col>
        <v-col md="4">
          <v-icon size="150" class="hidden-md-and-down">mdi-phone</v-icon>
        </v-col>
        <v-col md="4">
          <v-icon size="150" class="hidden-md-and-down">mdi-email</v-icon>
        </v-col>
      </v-row>
      <!--MOBILE ICONS POSITION -->
      <v-flex class="text-center my-5">
        <v-col>
          <v-icon size="100" class="hidden-md-and-up"
            >mdi-map-marker-radius</v-icon
          >
        </v-col>
        <v-col>
          <v-icon size="100" class="hidden-md-and-up">mdi-phone</v-icon>
        </v-col>
        <v-col>
          <v-icon size="100" class="hidden-md-and-up">mdi-email</v-icon>
        </v-col>
      </v-flex>
    </v-container>
  </div>
</template>
<script>
export default {
  name: "ContactView",
  components: {},
};
</script>
