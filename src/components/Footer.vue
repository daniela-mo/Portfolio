<template>
  <div class="footer">
    <strong
      >Desenvolvido por
      <a href="https://github.com/daniela-mo/Portfolio">Daniela Oliveira</a>
    </strong>
    <p>® Copyright 2022. Todos os Direitos Reservados.</p>
  </div>
</template>

<style lang="scss" scoped>
.footer {
  padding: 50px 0;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
  strong {
    font-weight: 300;
  }
  a {
    font-weight: 600;
    color: #9667aa;
  }
  a:hover {
    color: #9d0be0;
    transition: 0.3s;
  }
  @media (max-width: 500px) {
    align-items: center;
    justify-content: center;
    strong,
    p {
      font-size: 12px;
      font-weight: 300;
    }
    a {
      font-size: 12px;
      font-weight: 600;
      color: #9667aa;
    }
  }
}
</style>
