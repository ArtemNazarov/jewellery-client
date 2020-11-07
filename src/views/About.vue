<template>
  <section class="hero">
    <div class="hero-body">
      <div class="container">
        <h1 class="title">Jewellery</h1>
        <h2 class="subtitle">Awesome. Peerless. Comfortable.</h2>
      </div>
    </div>
  </section>
  <section class="hero is-light">
    <div class="hero-body">
      <div class="container">
        <h1 class="title">Новый взгляд</h1>
        <div class="columns">
          <div class="column" v-for="image in images" :key="image.src">
            <figure>
              <img v-bind:src="image.src" v-bind:alt="image.alt" />
            </figure>
          </div>
        </div>
        <h2 class="subtitle">На привычные вещи</h2>
      </div>
    </div>
  </section>
  <section class="hero is-info">
    <div class="hero-body">
      <div class="container">
        <h1 class="title">Рязань</h1>
        <h2 class="subtitle">Город, рождающий мечты</h2>
      </div>
    </div>
  </section>
</template>
<script>
export default {
  name: "About",
  data() {
    return {
      images: [
        {
          src:
            "https://sun1-25.userapi.com/PaIvt9ss1AGLfUrGddoRgZljLAdkxipVOuBgaA/BG8fD-UJtT4.jpg",
        },
        {
          src:
            "https://sun9-52.userapi.com/sIZKGZ5av9IbZYivkta_7wdmtn1h-ojtwkXT-g/M6F5ISATZbA.jpg",
        },
        {
          src:
            "https://sun1-94.userapi.com/xF6JoOoPCVe4Va4erWcOudY1NxWmh_I5aPw8RQ/Z040WGbEwwM.jpg",
        },
        {
          src:
            "https://sun9-46.userapi.com/_3cMkwPqcgT7R0-IsypjtoMOwebtSTjEgSFPWA/reJLxYmH3-k.jpg",
        },
      ],
    };
  },
};
</script>
<style scoped>
h1,
h2 {
  font-family: "Poppins", sans-serif;
}
h1 {
  letter-spacing: 2px;
}
h2 {
  letter-spacing: 1px;
}
</style>
