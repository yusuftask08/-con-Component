<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <BaseIcon name="success" width="45" height="40" />
    <BaseIcon name="error" width="45" height="40" />
    <BaseIcon name="info" width="45" height="40" />
  </div>
</template>

<script>
import BaseIcon from "./components/BaseIcon.vue";

export default {
  name: "App",
  components: {
    BaseIcon,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
}
</style>
