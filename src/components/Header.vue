<script>
  export default {};
</script>


<template>
    <header>
        <!-- Logo -->
        <a href="#" class="logo">Xae</a>
        <!-- Hamburger icon -->
        <input class="side-menu" type="checkbox" id="side-menu"/>
        <label class="hamb" for="side-menu">
          <span class="hamb-line"></span>
        </label>
        <!-- Menu -->
        <nav class="nav">
            <ul class="menu">
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Gallery</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>
</template>

<style>
a{
    text-decoration: none;
}

ul{
    list-style: none;
}

header{
  position: sticky;
  top: 0;
  height: 62px;
}

.logo{
  font-size: 4em;
  margin-left: 0.1em;
  color: black;
  font-weight: bold;
}

header div{
  display: flex;
}

.nav{
    width: 100%;
    height: 100%;
    position: fixed;
    overflow: hidden;
}
.menu a{
    display: flex;
    padding: 2em;
}
.menu a:hover{
    background-color: var(--gray);
}
.nav{
    max-height: 0;
    transition: max-height .5s ease-out;
}
.hamb{
    cursor: pointer;
    float: right;
    padding: 40px 20px;
}
.hamb-line {
    display: block;
    background: var(--black);
    height: 2px;
    position: relative;
    width: 24px;

} 
.hamb-line::before,
.hamb-line::after{
    background: var(--black);
    content: '';
    display: block;
    height: 100%;
    position: absolute;
    transition: all .2s ease-out;
    width: 100%;
}
.hamb-line::before{
    top: 5px;
}
.hamb-line::after{
    top: -5px;
}

.side-menu {
    display: none;
}
.side-menu:checked ~ nav{
    max-height: 100%;
}
.side-menu:checked ~ .hamb .hamb-line {
    background: transparent;
}
.side-menu:checked ~ .hamb .hamb-line::before {
    transform: rotate(-45deg);
    top:0;
}
.side-menu:checked ~ .hamb .hamb-line::after {
    transform: rotate(45deg);
    top:0;
}

</style>