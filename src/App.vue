<script>
import Header from "./components/HeaderComponent.vue";

export default {
  name: "app",
  components: {
    Header,
  },
};
</script>

<template>
  <Header />
  <main></main>
</template>

<style>
@import "./assets/base.css";
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@100&display=swap");

:root {
  --white: #f9f9f9;
  --black: #36383f;
  --gray: #85888c;
} /* variables*/

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background: rgb(41, 64, 73);
  background: linear-gradient(
    90deg,
    rgba(41, 64, 73, 1) 0%,
    rgba(0, 0, 0, 1) 100%
  );
  font-family: "Poppins", sans-serif;
}
</style>
