<template>
  <main class="container">
    <Header></Header>
    <SearchBar></SearchBar>
  </main>
</template>
<script>
import SearchBar from "./MainComponent/SearchBar";
import Header from "./MainComponent/Header";
export default {
  components: {
    SearchBar,
    Header
  },
  created() {
    this.fetchData();
  },
  methods: {
    async fetchData() {
      //   fetch("movies-coming-soon.json")
      //     .then(response => response.json())
      //     .then(commits => console.log(commits));
      //   fetch(
      //     `https://api.openweathermap.org/data/2.5/weather?q=pune&appid=4d8fb5b93d4af21d66a2948710284366&units=metric`
      //   )
      //     .then(response => response.json())
      //     .then(commits => console.log(commits));

      let response = await fetch("movies-coming-soon.json");
      let res = await response.json();
      console.log(res);
    }
  }
};
</script>
<style lang="scss" scoped>
main {
  width: 100%;
  height: 100px;
}
</style>
