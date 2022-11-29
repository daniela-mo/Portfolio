<template>
  <div class="presentation">
    <div>
      <img src="" alt="" />
      <h1 v-html="paper"></h1>
      <p class="presentation__desc texto">{{ description }}</p>

      <!-- <label class="label" for="check">
        <i class="fa-solid fa-moon" style="color#fff"></i>
        <i class="fa-solid fa-sun" style="color#fff"></i>
        <div class="btn"></div>
      </label> -->
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      h1: "Olá! Meu nome é Daniela =] ",
      description: "Desenvolvedora Front-end/Web ",
      paper: "",
      timer: null,
    };
  },

  mounted() {
    this.printer();
  },
  methods: {
    printer() {
      let i = -1;
      this.timer = setInterval(() => {
        i++;
        const x = i % this.h1.length;
        this.paper += this.h1[x];
      }, 300 - Math.random() * 50);
    },

    stoper() {
      clearInterval(this.timer);
      this.paper;
    },
  },
  watch: {
    paper: function () {
      if (this.paper.length == this.h1.length) {
        {
          this.stoper();
        }
      }
    },
  },
};
</script>

<style lang="scss" scoped>
.presentation {
  text-align: center;
  display: grid;
  /* grid-template-columns: 1fr; */
  column-gap: 30px;
  align-items: center;
  align-content: center;
  padding-bottom: 80px;
  h1 {
    font: bold 2.5rem/1.1 "Roboto Mono";
    margin-bottom: 20px;
    background: linear-gradient(to right, #a15dc0 30%, #9d0be0 70%);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  h1 {
    display: inline;
    border-right: 2px #9d0be0 solid;
    animation: typebar 0s steps(40) infinite;
  }
  .texto {
    margin-top: 5px;
    color: rgb(52, 52, 52);
  }
  p {
    font: 400 1rem "Roboto Mono", sans-serif;
    color: rgb(52, 52, 52);
  }
  @media (max-width: 500px) {
    flex-direction: column;
    padding: 0;
    width: 100%;
  }
}
</style>
