<template>
  <section class="subscribe">
    <h2>SUBSCRIBE</h2>
    <p class="subscribe__text">FOR OUR NEWLETTER AND PROMOTION</p>
    <form action="#" class="subscribe__form">
      <input
        class="subscribe__input-email"
        type="email"
        placeholder="Enter Your Email"
        minlength="3"
        maxlength="254"
        required
        v-model="value"
      /><button class="subscribe__input-submit" v-on:click="checkingEmail">
        SUBSCRIBE
      </button>
    </form>
  </section>
</template>

<script>
export default {
  name: "Subscribe",
  data() {
    return {
      value: "",
      regExp: /@/,
    };
  },
  methods: {
    checkingEmail() {
      if (!this.regExp.test(this.value)) {
        const $error = document.querySelector(".subscribe__input-email");
        $error.style.cssText = "border: 2px solid #F16D7F;";
      }
    },
  },
};
</script>