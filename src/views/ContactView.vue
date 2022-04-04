<template>
  <div class="contact">
    <v-container app>
      <v-layout column>
        <v-flex class="display-2 text-center my-5">Contact Us</v-flex>
        <p class="display-1 text-center my-5">Tell us what you need.</p>
      </v-layout>
      <v-row class="text-center my-5 hidden-md-and-down">
        <v-col md="4">
          <v-icon
            size="150"
            class="iconsStyle"
            onclick="window.open('https://www.google.com/maps/place/Atlantic+City,+NJ/@39.3766056,-74.4879282,13z/data=!4m5!3m4!1s0x89c0dd576e5cc721:0x4a6fcb43e9675262!8m2!3d39.3642834!4d-74.4229266')"
            >mdi-map-marker-radius</v-icon
          >
          <p
            class="iconsStyle"
            onclick="window.open('https://www.google.com/maps/place/Atlantic+City,+NJ/@39.3766056,-74.4879282,13z/data=!4m5!3m4!1s0x89c0dd576e5cc721:0x4a6fcb43e9675262!8m2!3d39.3642834!4d-74.4229266')"
          >
            Atlantic City, NJ, 08404
          </p>
        </v-col>
        <v-col md="4">
          <v-icon
            size="150"
            onclick="window.open('tel:609-436-2936');"
            class="iconsStyle"
            >mdi-phone</v-icon
          >
          <p onclick="window.open('tel:609-436-2936');" class="iconsStyle">
            609-436-2936
          </p>
        </v-col>
        <v-col md="4">
          <v-icon
            size="150"
            onclick="window.open('mailto:fully@clean.com');"
            class="iconsStyle"
            >mdi-email</v-icon
          >
          <p
            onclick="window.open('mailto:fully@clean.com');"
            class="iconsStyle"
          >
            fully@clean.com
          </p>
        </v-col>
      </v-row>
      <!--MOBILE ICONS POSITION -->
      <v-flex class="text-center my-5 hidden-md-and-up">
        <v-col>
          <v-icon
            class="iconsStyle"
            size="100"
            onclick="window.open('https://www.google.com/maps/place/Atlantic+City,+NJ/@39.3766056,-74.4879282,13z/data=!4m5!3m4!1s0x89c0dd576e5cc721:0x4a6fcb43e9675262!8m2!3d39.3642834!4d-74.4229266')"
            >mdi-map-marker-radius</v-icon
          >
          <p
            class="iconsStyle"
            onclick="window.open('https://www.google.com/maps/place/Atlantic+City,+NJ/@39.3766056,-74.4879282,13z/data=!4m5!3m4!1s0x89c0dd576e5cc721:0x4a6fcb43e9675262!8m2!3d39.3642834!4d-74.4229266')"
          >
            Atlantic City, NJ, 08404
          </p>
        </v-col>
        <v-col>
          <v-icon
            size="100"
            onclick="window.open('tel:609-436-2936');"
            class="iconsStyle"
            >mdi-phone</v-icon
          >
          <p onclick="window.open('tel:609-436-2936');" class="iconsStyle">
            609-436-2936
          </p>
        </v-col>
        <v-col>
          <v-icon
            size="100"
            class="iconsStyle"
            onclick="window.open('mailto:fully@clean.com');"
            >mdi-email</v-icon
          >
          <p
            class="iconsStyle"
            onclick="window.open('mailto:fully@clean.com');"
          >
            fully@clean.com
          </p>
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
<style>
.iconsStyle {
  cursor: pointer;
}
</style>
