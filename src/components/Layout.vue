<template>
  <Navbar />
  <main>
    <router-view />
  </main>
  <Footer />
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "Layout",
  components: {
    Navbar,
    Footer,
  },
};
</script>

<style>
*,
*:before,
*:after {
  box-sizing: border-box;
}

#app {
  display: flex;
  flex-direction: column;
  align-items: stretch;
  min-height: 100vh;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

main {
  flex-grow: 1;
}

header,
main,
footer {
  flex-shrink: 0;
}
</style>