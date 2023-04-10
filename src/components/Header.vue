<template>
    <nav class="header">
        <a href=""><img src="@/assets/logo-jr.png" alt="Logo" class="logo" /></a>
        <ul class="header-menu">
            <a href="" class="header-links">Home</a>
            <a href="#about" class="header-links">À propos</a>
            <a href="#projects" class="header-links">Projets</a>
        </ul>
    </nav>
</template>


<style scoped lang="scss">

ul {
  list-style: none;
  padding-inline-start: 0px;
}

.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #fff;
    font-size: 1rem;   
    padding: 15px 50px;
    max-width: var(--container-width);
    justify-items: center;
    margin: auto;

    @media screen and (max-width: 800px) {
        padding: 15px 30px;
    }
}


.header .logo {
    width: 100px;
    display: block;
}

.header-menu {
    display: flex;
    gap: 50px;

    @media screen and (max-width: 800px) {
        gap: 15px;
        font-size: 0.8rem;
    }
}


.header-links {
    color: var(--colors-black);;
    text-decoration: none;
    font-weight: normal;
    position: relative;

    &::after {
        content: "";
        position: absolute;
        bottom: -4px;
        left: 0;
        width: 0;
        height: 2px;
        background: var(--colors-blue);
        transition: all 300ms ease;
    }

    &:hover {
       &::after {
         width: 100%;
        }
    }
}
</style>