<script>
import LogoComponent from "./LogoComponent.vue";
import HamburguerComponent from "./HamburguerComponent.vue";
import MenuComponent from "./MenuComponent.vue";

export default {
  components: {
    LogoComponent,
    HamburguerComponent,
    MenuComponent,
  },
};
</script>

<template>
  <header>
    <LogoComponent />
    <HamburguerComponent />
    <MenuComponent />
  </header>
</template>

<style>
a {
  text-decoration: none;
  color: var(--white);
}

ul {
  list-style: none;
  align-items: center;
}

header {
  position: sticky;
  top: 0;
  height: 100%;
}

header div {
  display: flex;
}
</style>
