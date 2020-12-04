<template>
  <div id="app">
    <div id="nav">
      Sobre
    </div>
    <h1>Makeanote</h1>
    <p>A ideia é fazer um site onde seja possível adicionar notas que possam ser salvas na nuvem.
      <br>Eventualmente implementar também a possibilidade de exportar notas, e fazer alterações colaborativas!
    </p>
  </div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
