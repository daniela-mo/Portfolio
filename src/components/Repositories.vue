<template>
  <div class="container">
    <strong class="container__description"
      >Projetos criados para didática</strong
    >
    <h2 class="container__title">Repositórios</h2>
    <div class="container__projetos">
      <div class="container__projetos__repositorio">
        <h3>Clone da home Netflix</h3>
        <p>Tecnologias: HTML, CSS & JavaScript</p>

        <a href="https://github.com/daniela-mo/Clone-Netflix"
          >Link do Projeto</a
        >
      </div>
      <div class="container__projetos__repositorio">
        <h3>Game Play</h3>
        <p>Tecnologias: TypeScript & React Native</p>

        <a href="https://github.com/daniela-mo/GamePlay">Link do Projeto</a>
      </div>

      <div class="container__projetos__repositorio">
        <h3>Calculadora de Gorjetas</h3>
        <p>Tecnologias: Vue, HTML & JavaScript</p>

        <a href="https://github.com/daniela-mo/tipCalculator"
          >Link do Projeto</a
        >
      </div>
      <div class="container__projetos__repositorio">
        <h3>Clone do login Facebook</h3>
        <p>Tecnologias: Vue, HTML & JavaScript</p>

        <a href="https://github.com/daniela-mo/Clone-Facebook"
          >Link do Projeto</a
        >
      </div>
      <div class="container__projetos__repositorio">
        <h3>Planejando Viagens</h3>
        <p>Tecnologias: HTML, CSS & TypeScript</p>

        <a href="https://github.com/daniela-mo/places">Link do Projeto</a>
      </div>
      <div class="container__projetos__repositorio">
        <h3>Clima Tempo</h3>
        <p>Tecnologias: HTML, CSS & JavaScript</p>

        <a href="https://github.com/daniela-mo/Clone-Netflix"
          >Link do Projeto</a
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
.container {
  max-width: 1200px;
  margin: 0 auto;
  margin-top: 80px;
  &__description {
    font-size: 18px;
    font-weight: 400;
    color: rgb(52, 52, 52);
  }
  &__title {
    font: bold 1.8rem/1.1 "Roboto Mono";
    text-transform: uppercase;
    text-align: start;
    margin-bottom: 30px;
    margin-top: 5px;
    background: linear-gradient(to right, #a15dc0 30%, #9d0be0 70%);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }
  &__projetos {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    gap: 20px;
    justify-items: center;
    margin-bottom: 80px;
    &__repositorio {
      padding: 20px 30px;
      background: rgba(0, 0, 0, 0.2);
      box-shadow: 0 4px 5px rgba(0, 0, 0, 0.1);
      backdrop-filter: blur(4.8px);
      -webkit-backdrop-filter: blur(4.8px);
      border: 1px solid rgba(0, 0, 0, 0.22);
      display: flex;
      flex-direction: column;
      gap: 10px;
      a {
        color: #a15dc0;
      }
      h3 {
        font-size: 1.3rem;
        font-weight: bold;
        line-height: 1.1;
        /* transition: all 0.6s cubic-bezier(0.165, 0.84, 0.44, 1); */
      }
      h3:hover {
        font-size: 1.4rem;
        opacity: 50;
        cursor: pointer;
      }
    }
    &__repositorio:hover {
      color: rgb(52, 52, 52);
      /* background-color: #d4d0d0; */
      border: 1px solid #9d0be0;
    }
    &__repositorio a {
      /* background: linear-gradient(to left, #c19ed1 30%, #9d0be0 70%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent; */
      background: #79787833;
      display: inline-block;
      font-weight: 700;
      padding: 10px;
      text-align: center;
      border-radius: 4px;
      transition: all 0.6s cubic-bezier(0.165, 0.84, 0.44, 1);
    }
    &__repositorio a::after {
      opacity: 0;
      transition: all 0.3 cubic-bezier(0.165, 0.84, 0.44, 1);
    }
    &__repositorio a:hover {
      transform: scale(1.1);
      color: #9d0be0;
    }
    &__repositorio a:hover::after {
      opacity: 1;
    }
  }
  @media (max-width: 500px) {
    flex-direction: column;
    width: 100%;
    &__projetos {
      display: flex;
      flex-direction: column;
      margin-top: 50px;
    }
  }
}
</style>
