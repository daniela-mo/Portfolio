<template>
  <div class="header">
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
  justify-content: flex-end;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;

  &__menu {
    display: flex;
    margin-bottom: 50px;
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

  @media (max-width: 500px) {
    flex-direction: column;
    padding: 0;
    width: 100%;
    &__menu {
      margin: 10px 0 40px;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      li {
        padding: 0;
        margin: 0;
        border: 1px solid #9d0be0;
        border-radius: 4px;
        a {
          padding: 5px 10px;
          margin: 0;
        }
      }
    }
  }
}
</style>
