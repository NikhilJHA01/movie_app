<template>
  <div id="app">
    <MainComponent></MainComponent>
    <router-view />
  </div>
</template>

<script>
import MainComponent from "../src/components//MainComponent";
export default {
  data() {
    return {};
  },
  components: {
    MainComponent
  }
};
</script>

<style lang="scss">
@import "../src/styles/main.scss";
</style>
