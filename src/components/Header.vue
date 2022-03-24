<template>
  <div class="header">
    <p class="header__name">[DANIELA]</p>

    <nav>
      <ul class="header__menu">
        <li><a href="#projetos">Projetos</a></li>
        <li><router-link to="#social">Redes Sociais</router-link></li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.header {
  padding-top: 50px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
  &__name {
    background: linear-gradient(to right, #a744d4 30%, #9d0be0 70%);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    font-weight: bold;
    line-height: 1.1;
    font-size: 1.5rem;
  }
  &__menu {
    display: flex;
    gap: 30px;
  }
  &__menu a {
    display: inline-block;
    padding: 16px 0px;
    color: #a15dc0;
  }
  &__menu a::before {
    /* content: ""; */
    display: block;
    width: 0%;
    height: 2px;
    background: linear-gradient(to right, #a15dc0 30%, #9d0be0 70%);
    margin-top: 4px;
    position: absolute;
    text-decoration: none;
  }
  &__menu a::after {
    content: "";
    display: block;
    width: 0%;
    height: 2px;
    background: linear-gradient(to right, #a15dc0 30%, #9d0be0 70%);
    margin-top: 4px;

    text-decoration: none;
  }
  &__menu a:hover::after {
    width: 100%;
    transition: 0.3s;
  }
}
</style>
