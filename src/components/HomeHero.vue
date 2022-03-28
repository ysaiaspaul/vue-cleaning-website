<template>
  <v-container fluid fill-height class="home-hero" style="max-height: 100vh">
    <v-layout justify-center align-center column pa-5>
      <div class="ma-12 display-3 font-weight-black white--text text-xs-center">
        REQUEST A FREE
      </div>
      <div class="display-3 font-weight-black white--text text-xs-center mb-3">
        ESTIMATE
      </div>
      <v-flex>
        <Form></Form>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
import Form from "@/components/Form";
export default {
  name: "HomeHero",
  components: {
    // eslint-disable-next-line vue/no-unused-components
    Form,
  },
};
</script>

<style scoped>
.home-hero {
  background: url("https://images.unsplash.com/photo-1563453392212-326f5e854473?crop=entropy&cs=srgb&fm=jpg&ixid=MnwxNDU4OXwwfDF8cmFuZG9tfHx8fHx8fHx8MTY0NjgwMTQ0OQ&ixlib=rb-1.2.1&q=85");
  background-size: cover;
  width: 100%;
  height: 100%;
}
</style>
