<template>
  <div id="app">
    <home />
  </div>
</template>

<script>
import home from "../src/pages/home";

export default {
  name: "Home",
  components: {
    home,
  },
};
</script>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

</style>
