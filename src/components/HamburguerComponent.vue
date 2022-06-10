<script>
export default {};
</script>

<template>
  <input class="side-menu" type="checkbox" id="side-menu" />
  <label class="hamb" for="side-menu">
    <span class="hamb-line"></span>
  </label>
</template>

<style>
.hamb {
  cursor: pointer;
  float: right;
  padding: 40px 20px;
}
.hamb-line {
  display: block;
  background: var(--white);
  height: 2px;
  position: relative;
  width: 24px;
}
.hamb-line::before,
.hamb-line::after {
  background: var(--white);
  content: "";
  display: block;
  height: 100%;
  position: absolute;
  transition: all 0.2s ease-out;
  width: 100%;
}
.hamb-line::before {
  top: 5px;
}
.hamb-line::after {
  top: -5px;
}

.side-menu {
  display: none;
}
.side-menu:checked ~ nav {
  max-height: 100%;
}
.side-menu:checked ~ .hamb .hamb-line {
  background: transparent;
}
.side-menu:checked ~ .hamb .hamb-line::before {
  transform: rotate(-45deg);
  top: 0;
}
.side-menu:checked ~ .hamb .hamb-line::after {
  transform: rotate(45deg);
  top: 0;
}
</style>
