<template>
  <Navbar />
  <Header />
  <About />
</template>

<script>
import Navbar from "./Navbar.vue";
import Header from "./Header.vue";
import About from "./About.vue";

export default {
  name: "Home",
  data() {
    return {};
  },

  components: {
    Navbar,
    Header,
    About,
  },
};
</script>

<style></style>
