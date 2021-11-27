<template>
  <div class="container">
    <Navbar />
    <Hero />
    <HomeBody />
    <div class="container center-block text-center">
      <center>
        <div class="best-products">
          <div class="row mb-4">
            <div
              class="col-md-4 mt-4"
              v-for="product in products"
              :key="product.id"
            >
              <CardProduct :product="product" />
            </div>
          </div>
        </div>
      </center>
      <router-link to="/foods"
        ><button type="button" class="btn btn-outline-success mt-5 mb-5">
          Lihat semua <b-icon icon="arrow-right"></b-icon></button
      ></router-link>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";
import Hero from "@/components/Hero.vue";
import HomeBody from "@/components/HomeBody.vue";
import CardProduct from "@/components/CardProduct.vue";
import axios from "axios";

export default {
  name: "Home",
  components: {
    Navbar,
    Hero,
    HomeBody,
    CardProduct,
  },
  data() {
    return {
      products: [],
    };
  },
  methods: {
    setProduct(data) {
      this.products = data;
    },
  },
  mounted() {
    axios
      .get("http://localhost:3000/best-products")
      .then((response) => this.setProduct(response.data))
      .catch((error) => console.log(error));
  },
};
</script>
