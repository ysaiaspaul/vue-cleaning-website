<template>
  <v-app>
    <v-app-bar app color="white">
      <v-toolbar-title style="color: black">{{ appTitle }}</v-toolbar-title>
      <v-toolbar color="white" flat>
        <v-tabs v-model="activeTab" left slider-color="#5b5b5b" class="ml-16">
          <v-tab
            v-for="tab of tabs"
            :key="tab.id"
            :to="tab.route"
            exact
            style="color: #5b5b5b"
          >
            {{ tab.name }}
          </v-tab>
        </v-tabs>
        <v-btn depressed right color="#0397D9" class="white--text"
          >Pricing</v-btn
        >
      </v-toolbar>
    </v-app-bar>
    <v-content>
      <v-fade-transition>
        <router-view></router-view>
      </v-fade-transition>
    </v-content>
    <Footer></Footer>
  </v-app>
</template>

<style></style>
<script>
import Footer from "@/components/Footer";
export default {
  name: "App",
  props: ["id"],
  data() {
    return {
      appTitle: "Fully Clean",
      activeTab: "/app/${this.id}",
      tabs: [
        { id: 1, name: "Home", route: "/" },
        { id: 2, name: "About", route: "/about" },
        { id: 3, name: "Contact Us", route: "/contactUs" },
      ],
    };
  },
  components: { Footer },
};
</script>
