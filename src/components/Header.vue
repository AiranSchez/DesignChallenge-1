<script>
import Logo from './Logo.vue'
import Hamburger from './Hamburguer.vue'
import Menu from './Menu.vue'

export default {
    components: {
        Logo,
        Hamburger,
        Menu
    }
};
</script>


<template>
    <header>
        <Logo/>
        <Hamburger/>
        <Menu/>
    </header>
</template>

<style>
a{
    text-decoration: none;
    color: var(--white)
}

ul{
    list-style: none;
    align-items: center;
}

header{
  position: sticky;
  top: 0;
  height: 100%;
}

header div{
  display: flex;
}

</style>