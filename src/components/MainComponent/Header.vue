<template>
  <header class="container">
    <h1 class="title">Assignment Name</h1>
    <i class="fa fa-camera-retro"></i>
    <i class="fa fa-refresh fa-spin fa-3x fa-fw" aria-hidden="true"></i>
    <span class="sr-only">Refreshing...</span>
    <a class="btn btn-default" href="" aria-label="Settings">
      <i class="fa fa-cog" aria-hidden="true"></i>
      <i class="fa fa-trash" aria-hidden="true"></i>
    </a>
  </header>
</template>
<script>
export default {
  name: "Header"
};
</script>
<style lang="scss" scoped>
header {
  height: 10vh;
  background-color: blue;
  display: flex;
  align-items: center;
  justify-content: flex-start;

  .title {
    font-size: 2rem;
    color: white;
  }
}
</style>
