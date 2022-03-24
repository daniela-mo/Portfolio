<template>
  <div id="app">
    <router-view />
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
  list-style: none;
}

body {
  background: #171717;
  font-family: "Roboto Mono", "Roboto";
  color: #f9f9f9;
  transition: background 0.2s linear;
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
