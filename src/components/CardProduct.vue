<template>
  <div>
    <div class="card shadow rounded">
      <img
        :src="' ../assets/images/' + product.gambar"
        class="card-img-top"
        alt="Card image cap"
      />
      <div class="card-body">
        <h5 class="card-title">{{ product.nama }}</h5>
      </div>
      <ul class="list-group list-group-flush">
        <li class="list-group-item">Harga: {{ product.harga }}</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardProduct",
  props: ["product"],
};
</script>

<style>
</style>