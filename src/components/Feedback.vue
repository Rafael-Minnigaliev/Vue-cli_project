<template>
  <aside class="feedback center">
    <section class="reviews">
      <h2 class="hidden">reviews</h2>
      <picture>
        <source srcset="img/reviews-photo.webp" type="image/webp" />
        <img
          src="img/reviews-photo.png"
          class="reviews__photo"
          alt="photo"
        /> </picture
      ><br />
      “Vestibulum quis porttitor dui! Quisque viverra nunc mi,
      <span class="reviews__text">a pulvinar purus condimentum“</span>
    </section>
    <Subscribe />
  </aside>
</template>


<script>
import Subscribe from "@/components/Subscribe.vue";

export default {
  name: "Feedback",
  components: {
    Subscribe,
  },
};
</script>