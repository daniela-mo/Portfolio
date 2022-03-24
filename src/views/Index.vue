<template>
  <div class="home">
    <Header />
    <Presentation />
    <Home />
    <Social />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Header from "@/components/Header";
import Presentation from "@/components/Presentation";
import Home from "@/components/Home.vue";
import Social from "@/components/Social.vue";
import Footer from "@/components/Footer.vue";

export default {
  components: {
    Header,
    Presentation,
    Home,
    Social,
    Footer,
  },
};
</script>
