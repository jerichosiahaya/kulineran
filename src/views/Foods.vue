<template>
  <div class="container">
    <Navbar />
    <Hero />
    <h2 class="text-center mt-4">Daftar Makanan</h2>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";
import Hero from "@/components/Hero.vue";

export default {
  name: "Foods",
  components: {
    Navbar,
    Hero,
  },
};
</script>

<style>
</style>