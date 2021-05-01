<template>
  <nav class="searchBar container">
    <form @submit.prevent="searchResults()">
      <input type="text" placeholder="Search for a city" autofocus />
      <button type="submit">SUBMIT</button>
      <span class="msg"></span>
    </form></nav
></template>
<script>
export default {
  name: "SearchBar",
  methods: {
    searchResults() {
      alert("hello");
    }
  }
};
</script>
<style lang="scss" scoped>
.searchBar {
  color: #fff;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 20vh;

  form {
    position: relative;
    display: flex;

    input {
      font-size: 2rem;
      height: 40px;
      padding: 5px 5px 10px;
      border-bottom: 1px solid black;
      color: black;
    }
    input::placeholder {
      color: black;
    }
    button {
      font-size: 1rem;
      font-weight: bold;
      letter-spacing: 0.1em;
      padding: 15px 20px;
      margin-left: 15px;
      border-radius: 5px;
      background: red;
      transition: background 0.3s ease-in-out;
    }
    button:hover {
      background: #c3112d;
    }
    .msg {
      position: absolute;
      bottom: -40px;
      left: 0;
      max-width: 450px;
      min-height: 40px;
      font-size: 1rem;
      padding: 10px;
    }
  }
}
</style>
