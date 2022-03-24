<template>
  <div class="home">
    <Home msg="Welcome to Your Vue.js App" />
    <h2>Home</h2>
  </div>
</template>

<script>
// @ is an alias to /src
import Home from "@/components/Home.vue";

export default {
  name: "HomeView",
  components: {
    Home,
  },
};
</script>
