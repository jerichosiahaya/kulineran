<template>
  <div>
    <div class="card shadow" style="width: 18rem">
      <img
        :src="' ../assets/images/' + product.gambar"
        class="card-img-top"
        alt="Card image cap"
      />
      <div class="card-body">
        <h5 class="card-title">{{ product.nama }}</h5>
        <p class="card-text">Harga: {{ product.harga }}</p>
        <a href="#" class="btn btn-success"
          ><b-icon icon="cart3"></b-icon> Pesan</a
        >
      </div>
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