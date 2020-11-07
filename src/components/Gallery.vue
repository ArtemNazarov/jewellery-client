<template>
  <section class="section">
    <div class="container">
      <div class="columns is-multiline">
        <div v-for="image in images" class="column" :key="image.src">
          <figure>
            <img v-bind:src="image.src" v-bind:alt="image.alt" />
          </figure>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Gallery",
  data() {
    return {
      images: [
        {
          src:
            "https://sun9-54.userapi.com/zHAr3BYYNla8Wj8lXTcANYieQ9tM8NcjrSs_EQ/VjI_7vG4nSk.jpg",
        },
        {
          src:
            "https://sun9-36.userapi.com/c858528/v858528491/1ae22d/t8DnGDj3YzY.jpg",
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
            "https://sun1-25.userapi.com/PaIvt9ss1AGLfUrGddoRgZljLAdkxipVOuBgaA/BG8fD-UJtT4.jpg",
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

<style>
</style>