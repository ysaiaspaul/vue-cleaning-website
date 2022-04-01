<template>
  <div class="home">
    <HomeHero app></HomeHero>
    <v-container app>
      <v-layout column>
        <v-flex class="display-2 text-center my-5">Who we are</v-flex>
        <v-flex>
          <div class="headline mt-3">Fully clean</div>
          <p class="subheading mt-3">Loren ipsum dolor sit amet, consectetur</p>
        </v-flex>
        <v-flex>
          <div class="headline mt-3">Loren ipsum</div>
          <p>Loren ipsum dolor sit amet, consectetur</p>
          <p class="subheading mt-3">
            Nulls nec massa eu est fringilla lobortis. Praesent in enum in justo
            in justo blandit varius. Cras placerat arcu in sapiens rhoncus
            rhoncus aliquet. Sed interdum tortor et incident condimentum. Etiam
            consequat mi leo, in suscipit odio scelerisque molestie. Nam et
            purus consequat, iaculis augue augue vel, sagittis ligula.
            Vestibulum aliquet vulputate erat. Phasellus id mauris mauris. Nunc
            a maximus dolor. Curator ut ut vestibulum arcu. Curabitur non lacus
            justo. Cras varius a magna in semper. Nulla eros ante, consectetur
            faucibus.
          </p>
          <p class="subheading mt-3">
            Nulls nec massa eu est fringilla lobortis. Praesent in enum in justo
            in justo blandit varius. Cras placerat arcu in sapiens rhoncus
            rhoncus aliquet. Sed interdum tortor et condimentum. Etiam consequat
            mi leo, in suscipit odio scelerisque molestie. Nam et purus
            consequat, iaculis augue augue vel, sagittis ligula. Vestibulum
            aliquet vulputate erat. Phasellus id mauris mauris. Nunc a maximus
            dolor. Curator ut ut vestibulum arcu. Curabitur non lacus justo.
            Cras varius a magna in semper. Nulla eros ante, consectetur
            faucibus.
          </p>
        </v-flex>
        <v-flex>
          <div class="headline mt-3">Loren ipsum</div>
          <p class="subheading mt-3">
            Nulls nec massa eu est fringilla lobortis. Praesent in enum in justo
            in justo blandit varius. Cras placerat arcu in sapiens rhoncus
            rhoncus aliquet. Sed interdum tortor et incident condimentum. Etiam
            consequat mi leo, in suscipit odio scelerisque molestie. Nam et
            purus consequat, iaculis augue augue vel, sagittis ligula.
            Vestibulum aliquet vulputate erat. Phasellus id mauris mauris. Nunc
            a maximus dolor. Curator ut ut vestibulum arcu. Curabitur non lacus
            justo. Cras varius a magna in semper. Nulla eros ante, consectetur
            faucibus faucibus faucibus faucibus sapiens eu, rhoncus imperdiet
            dui.
          </p>
        </v-flex>
        <v-flex class="display-2 text-center my-16"
          >What Our Clients Say?</v-flex
        >
        <v-flex mb-16>
          <testimonials></testimonials>
        </v-flex>
        <v-flex class="display-2 text-center my-10"
          >Give Us A Call Today
        </v-flex>
        <v-layout justify-center mb-16>
          <Form></Form>
        </v-layout>
      </v-layout>
    </v-container>
  </div>
</template>

<script>
// @ is an alias to /src
import Form from "@/components/Form";
import HomeHero from "@/components/HomeHero";
import Testimonials from "@/components/Testimonials";
export default {
  name: "HomeView",
  components: {
    HomeHero,
    Testimonials,
    Form,
  },
};
</script>
