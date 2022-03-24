<template>
  <div class="home">
    <Header />
    <Presentation />
    <Home />
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

<style lang="scss" scoped>
.home {
  @media (max-width: 500px) {
    margin: 0 20px;
    /* align-items: center; */
  }
}
#back-to-top {
  cursor: pointer;
  display: none;
  justify-content: center;
  align-items: center;
  width: 35px;
  height: 35px;
  position: fixed;
  bottom: 15px;
  left: 1450px;
  background-color: black;
  border-radius: 20px;
  color: #f9f9f9;
  transition: 0.3s;
  z-index: 1;
}
#back-to-top i {
  font-size: 20px;
}
</style>
