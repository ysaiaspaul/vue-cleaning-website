<template>
  <v-app>
    <v-app-bar app color="red lighten-3" dark>
      <v-toolbar-title>{{ appTitle }}</v-toolbar-title>
      <v-toolbar color="red lighten-3" dark flat>
        <v-tabs v-model="activeTab" centered>
          <v-tab v-for="tab of tabs" :key="tab.id" :to="tab.route" exact>
            {{ tab.name }}
          </v-tab>
        </v-tabs>
      </v-toolbar>
    </v-app-bar>
    <v-main>
      <v-container fluid>
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
