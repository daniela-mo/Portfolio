<template>
  <div class="header">
    <div>
      <span>
        <strong>{{ name }}</strong> /></span
      >
    </div>
    <Toggle />
    <nav>
      <ul class="header__menu">
        <li><a href="#projetos">Projetos</a></li>
        <li><a href="#projetos">Aprensentação</a></li>
        <li><a href="#projetos">Projetos</a></li>
        <li><router-link to="#social">Redes Sociais</router-link></li>
      </ul>
    </nav>
  </div>
</template>

<script>
import Toggle from "@/components/common/Toggle.vue";
export default {
  data() {
    return {
      name: "Daniela Oliveira",
    };
  },

  components: {
    Toggle,
  },
};
</script>

<style lang="scss" scoped>
.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  border: 2px solid yellow;
  max-width: 1440px;
  margin: 50px 20%;
  span {
    font-weight: bold;
    color: #000;
  }
  &__menu {
    display: flex;
    gap: 30px;
    ul {
      li {
        a {
          display: inline-block;
          padding: 16px 0;
        }
      }
    }
  }
}
</style>
