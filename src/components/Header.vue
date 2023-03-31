<template id="header">
    <nav class="header">
        <a href=""><img src="@/assets/logo-jr.png" alt="Logo" class="logo" /></a>
        <ul class="header-menu">
            <a href="" class="header-links">Home</a>
            <a href="#resume" class="header-links">About</a>
            <a href="#projects" class="header-links">Projects</a>
        </ul>
    </nav>
</template>


<style scoped>

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
    /* position: sticky;
    top: 0;
    z-index: 1; */
    padding: 15px 0px 15px 0px;
    max-width: 1174px;
    justify-items: center;
    margin: auto;
}

.header .logo {
    width: 100px;
    display: block;
}

.header-menu {
    display: flex;
    gap: 50px;
}

.header-links {
    color: #1E1E1E;
    text-decoration: none;
    font-weight: normal;
    position: relative;
}

.header-links::after {
    content: "";
    position: absolute;
    bottom: -4px;
    left: 0;
    width: 0;
    height: 2px;
    background: #11b2cc;
    transition: all 300ms ease;
}

.header-links:hover::after {
    width: 100%;
}

</style>