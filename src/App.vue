<template>
  <div id="app">
    <router-view />
  </div>
</template>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@100;200;300;400;500;600;700;800;900&display=swap");
#app {
  font-family: "Montserrat", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  a:hover,
  a:focus {
    text-decoration: none;
  }
}
.title-main {
  margin-bottom: 45px;
  h2 {
    font-size: 36px;
    color: #0e3e62;
    font-weight: 600;
    padding: 0;
    margin: 0 0 30px 0;
  }
  span {
    font-size: 16px;
    color: #6e7377;
    font-weight: 500;
    padding: 0;
    margin: 0;
  }
}
</style>
