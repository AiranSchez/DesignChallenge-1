<script setup lang="ts">

</script>

<template>
  <header>
    <div id="title">Xae</div>
      <input class="side-menu" type="checkbox" id="side-menu"/>
      <!-- Hamburger icon -->
      <label class="hamb" for="side-menu">
        <span class="hamb-line"></span>
      </label>
      <!-- Menu -->
      <nav class="nav">
          <ul class="menu">
              <li><a href="#">Gallery</a></li>
              <li><a href="#">Blog</a> </li>
              <li><a href="#">About</a></li>
          </ul>
      </nav>
  </header>
</template>

<style>
@import './assets/base.css';
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100&display=swap');

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  
}

body {
  font-family: "Poppins", sans-serif;
}

header{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  height: 62px;
}

#title{
  font-size: 2em;
  color: black;
  font-weight: bold;
}

header div{
  display: flex;
}

.hamburguer{
  background-color: transparent;
  border: none;
  outline: none;
  cursor: pointer;
}

.hamburguer .line{
  display: block;
  width: 40px;
  height: 3px;
  background-color: #ecf0f1;
  margin-block: 10px;
  border-radius: 4px;
  transition: transform .5s, opacity .25s;
}

.hamburguer.active .line:nth-child(1){
  transform: translateY(13px) rotate(45deg);
}

.hamburguer.active .line:nth-child(2){
  opacity: 0;
}

.hamburguer.active .line:nth-child(3){
  transform: translateY(-13px) rotate(-45deg);
}

</style>
