<template>
  <v-app>
    <v-app-bar app color="blue lighten-4">
      <v-toolbar-title style="color: black">{{ appTitle }}</v-toolbar-title>
      <v-toolbar color="blue lighten-4" flat>
        <v-tabs v-model="activeTab" centered slider-color="#5b5b5b">
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
      </v-toolbar>
    </v-app-bar>
    <v-content transition="slide-x-transition">
      <router-view></router-view>
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
      ],
    };
  },
  components: { Footer },
};
</script>
