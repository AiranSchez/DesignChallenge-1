<script>
import Header from './components/Header.vue'

export default {
  name: 'app',
  components: {
    Header
  }
};
</script>

<template>
  <Header />
  <main></main>
</template>

<style>
@import './assets/base.css';
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100&display=swap');
  
:root{
    --white: #f9f9f9;
    --black: #36383F;
    --gray: #85888C;
} /* variables*/

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  
}

body {
  background-color: var(--white);
  font-family: "Poppins", sans-serif;
}

</style>
