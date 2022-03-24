<template>
  <div class="home">
    <HomeHero app></HomeHero>
    <v-container app>
      <v-layout column>
        <v-flex class="display-2 text-xs-center my-5">Fully Clean</v-flex>
        <v-flex>
          <div class="headline mt-3">Loren ipsum</div>
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
      </v-layout>
    </v-container>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeHero from "@/components/HomeHero";
export default {
  name: "HomeView",
  components: {
    HomeHero,
  },
};
</script>
