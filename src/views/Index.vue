<template>
  <div class="home">
    <Header />
    <Presentation />
    <Repositories />
    <Social />
    <Footer />
    <!-- <div id="back-to-top">
      <i class="fas fa-arrow-up"></i>
    </div> -->
  </div>
</template>

<script>
import Header from "@/components/Header";
import Presentation from "@/components/Presentation";
import Repositories from "@/components/Repositories.vue";
import Social from "@/components/Social.vue";
import Footer from "@/components/Footer.vue";

export default {
  components: {
    Header,
    Presentation,
    Repositories,
    Social,
    Footer,
  },
};
</script>

<style lang="scss" scoped>
.home {
  @media (max-width: 500px) {
    margin: 0 20px;
    /* align-items: center; */
  }
}
</style>
