<template>
  <v-app dark>
    <Navbar />
    <v-main>
      <nuxt />
    </v-main>
    <Footer />
  </v-app>
</template>

<script>
import Navbar from "~/components/Navbar";
import Footer from "~/components/Footer";
export default {
  components: {
    Navbar,
    Footer
  },
  data() {
    return {};
  }
};
</script>
<style lang="scss">
:root {
  --primary-color: #ffb610;
  --dark-color: #121212;
}
h2 {
  font-size: 2rem;
  position: relative;
  &:before {
    position: absolute;
    content: "";
    background-color: var(--primary-color);
    bottom: -0.5rem;
    left: 0;
    width: 70px;
    border-radius: 10px;
    height: 10px;
  }
}
a {
  text-decoration: none;
}
.container {
  @media (max-width: 1055px) {
    width: 80% !important;
  }
}
</style>
