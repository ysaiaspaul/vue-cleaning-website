<template>
  <v-app>
    <v-app-bar app color="red lighten-4">
      <v-toolbar-title style="color: black">{{ appTitle }}</v-toolbar-title>
      <v-toolbar color="red lighten-4" flat>
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
    <v-main>
      <v-container transition="slide-x-transition">
        <router-view></router-view>
      </v-container>
    </v-main>
  </v-app>
</template>

<style></style>
<script>
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
};
</script>
