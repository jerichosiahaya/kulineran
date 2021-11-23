<template>
  <div>
    <b-carousel
      id="carousel-no-animation"
      style="text-shadow: 0px 0px 2px #000"
      no-animation
      indicators
      img-width="1024"
      img-height="480"
    >
      <b-carousel-slide
        caption="Text Goes Here"
        img-src="https://picsum.photos/1024/480/?image=10"
      ></b-carousel-slide>
      <b-carousel-slide
        caption="Text Goes Here"
        img-src="https://picsum.photos/1024/480/?image=12"
      ></b-carousel-slide>
      <b-carousel-slide
        caption="Text Goes Here"
        img-src="https://picsum.photos/1024/480/?image=22"
      ></b-carousel-slide>
      <b-carousel-slide
        caption="Text Goes Here"
        img-src="https://picsum.photos/1024/480/?image=23"
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