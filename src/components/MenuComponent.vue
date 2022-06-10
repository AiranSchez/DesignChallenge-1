<script>
export default {};
</script>

<template>
  <nav class="nav">
    <ul class="menu">
      <li><a href="#">Home</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#">Gallery</a></li>
      <li><a href="#">Contact</a></li>
    </ul>
  </nav>
</template>

<style>
.nav {
  width: 100%;
  height: 100%;
  position: fixed;
  overflow: hidden;
}
.menu a {
  display: flex;
  justify-content: center;
  padding: 2em;
}
.menu li a {
  color: var(--white);
  font-size: 1em;
  font-weight: bold;
}
.menu a:hover {
  background-color: var(--gray);
}
.nav {
  max-height: 0;
  transition: max-height 0.5s ease-out;
}
</style>
