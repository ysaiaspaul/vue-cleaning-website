<template>
  <v-app>
    <v-navigation-drawer
      app
      v-model="drawer"
      class="blue lighten-5"
      disable-watcher
      temporary
    >
      <v-list nav dense>
        <v-list-item v-for="tab of tabs" :key="tab.id" :to="tab.route">
          <v-spacer :key="tab.id"></v-spacer>
          <v-list-title :key="id">
            <v-list-title-content style="color: black">
              <v-list-item-title>
                {{ tab.name }}
              </v-list-item-title>
            </v-list-title-content>
          </v-list-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar app color="white">
      <v-app-bar-nav-icon
        class="hidden-md-and-up"
        style="color: black"
        @click.stop="drawer = !drawer"
      >
      </v-app-bar-nav-icon>
      <v-spacer class="hidden-md-and-up"></v-spacer>
      <v-toolbar-title style="color: black">{{ appTitle }}</v-toolbar-title>
      <!-- DESKTOP MENU -->
      <v-toolbar color="white" flat>
        <v-tabs
          v-model="activeTab"
          left
          slider-color="#5b5b5b"
          class="ml-16 hidden-md-and-down"
        >
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
        <v-spacer class="hidden-md-and-up"></v-spacer>
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
      drawer: false,
      group: null,
      appTitle: "Fully Clean",
      activeTab: "/app/${this.id}",
      watch: {
        group() {
          this.drawer = false;
        },
      },
      tabs: [
        { id: 1, name: "Home", route: "/" },
        { id: 2, name: "About", route: "/about" },
        { id: 3, name: "Contact Us", route: "/contact" },
      ],
    };
  },
  components: { Footer },
};
</script>
