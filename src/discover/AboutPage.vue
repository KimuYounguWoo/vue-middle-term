<template>
  <Navbar />

  <div class="hidden lg:block container mt-5">
    <div class="page-banner1">
      <div class="row justify-content-center align-items-center h-100">
        <div class="col-md-6">
          <nav aria-label="Breadcrumb">
            <ul class="breadcrumb justify-content-center py-0 bg-transparent">
              <li class="breadcrumb-item">
                <router-link to="/">Home</router-link>
              </li>
              <li class="breadcrumb-item active">About</li>
            </ul>
          </nav>
          <h1 class="text-center">About Us</h1>
        </div>
      </div>
    </div>
  </div>
  <About />
</template>

<script>
import Navbar from "../components/Navbar";
import About from "../components/About";

export default {
  name: "About Page",
  data() {
    return {};
  },

  props: {
    blog: Array,
  },

  components: {
    Navbar,
    About,
  },
};
</script>

<style></style>
