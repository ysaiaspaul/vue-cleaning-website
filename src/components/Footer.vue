<template>
  <v-footer color="blue lighten-4" padless>
    <v-row justify="center" no-gutters>
      <v-btn
        v-for="link of links"
        :key="link.id"
        :to="link.route"
        color="#5b5b5b"
        text
        rounded
        class="my-2"
      >
        {{ link.name }}
      </v-btn>
      <v-col class="blue lighten-4 py-4 text-center #5b5b5b--text" cols="12">
        {{ new Date().getFullYear() }} - <strong>Fully Clean</strong>
      </v-col>
    </v-row>
  </v-footer>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Footer",
  data() {
    return {
      activeTab: "/app/${this.id}",
      links: [
        { id: 1, name: "Home", route: "/" },
        { id: 2, name: "About", route: "/about" },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
