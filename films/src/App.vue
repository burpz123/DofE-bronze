<template>
  <div id="app">
    <div class="container">
      <div class="row">
        <div class="col-sm">
          <film-list />
        </div>
        <div class="col-sm">
          <p>detail</p>
          <film-detail />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import FilmDetail from "./components/FilmDetail.vue";
import FilmList from "./components/FilmList.vue";

export default {
  name: "App",
  components: {
    FilmDetail, FilmList
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
