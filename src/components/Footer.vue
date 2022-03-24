<template>
  <div class="footer">
    <strong>Desenvolvido por <span>Daniela Oliveira</span> </strong>
    <p>® Copyright 2022. Todos os Direitos Reservados.</p>
  </div>
</template>

<style lang="scss" scoped>
.footer {
  padding-top: 50px;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
  strong {
    font-weight: 300;
  }
  span {
    font-weight: 600;
    color: #9667aa;
  }
  span:hover {
    color: #9d0be0;
    transition: 0.3s;
  }
}
</style>
