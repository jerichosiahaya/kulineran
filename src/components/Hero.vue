<template>
  <div>
    <b-carousel
      id="carousel-no-animation"
      style="text-shadow: 0px 0px 2px #000"
      no-animation
      indicators
      img-width="1024"
      img-height="280"
    >
      <b-carousel-slide
        caption="Text Goes Here"
        img-src="assets/images/header-1.jpg"
      ></b-carousel-slide>
      <b-carousel-slide
        caption="Text Goes Here"
        img-src="assets/images/header-2.jpg"
      ></b-carousel-slide>
      <b-carousel-slide
        caption="Text Goes Here"
        img-src="assets/images/header-3.jpg"
      ></b-carousel-slide>
      <b-carousel-slide
        caption="Text Goes Here"
        img-src="assets/images/header-4.jpg"
      ></b-carousel-slide>
    </b-carousel>
  </div>
</template>

<script>
export default {
  name: "Hero",
};
</script>

<style>
</style>