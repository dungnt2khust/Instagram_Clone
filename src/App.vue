<template>
  <div id="app">
    <div class="wrapper d-flex flex-row justify-content-center">
      <div class="header">
        <Header />
      </div>
    </div>
    <hr class="m-0 w-100" />
    <div class="d-flex flex-row">
      <div class="main">
        <OnlineUsers class="m-t-20" />
      </div>
    </div>
  </div>
</template>

<script>
import Header from "./layouts/Header";
import OnlineUsers from "./layouts/OnlineUsers";
export default {
  name: "App",
  components: { Header, OnlineUsers },
};
</script>

<style lang="scss">
@import "./assets/css/main.scss";
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 100vw;
  height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  .wrapper {
    width: 100%;
  }
}
</style>
