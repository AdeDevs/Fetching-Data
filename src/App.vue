<template>
  <div class="app-container">
    <HomePage msg="With Alt" />
  </div>
</template>

<script>
import HomePage from "./components/HomePage.vue";
export default {
  name: "App",
  components: {
    HomePage,
  },
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
}

.app-container {
  margin: 5px auto;
  width: 98%;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
