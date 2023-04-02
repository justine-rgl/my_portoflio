<template id="footer">
        <nav class="footer">
        <ul class="buttons">
            <a href="mailto:justine.rougeulle@gmail.com" class="contact">Contactez-moi !</a>
            <a href="https://github.com/justine-rgl" target="_blank" class="github"><img src="@/assets/github_white.png" alt="GitHub" class="icon"></a>
            <a href="https://www.linkedin.com/in/justinerougeulle/" target="_blank" class="linkedin"><img src="@/assets/linkedin_white.png" alt="Linkedin" class="icon"></a>
            <a href="https://www.youtube.com/watch?v=dQw4w9WgXcQ&ab" target="_blank" class="heart"><img src="@/assets/heart_white.png" alt="Coeur" class="icon"></a>
        </ul>
        <a href="#" v-scroll-to="'#header'"><img src="@/assets/logo-jr-footer.png" alt="logo" class="logo" /></a>
    </nav>
</template>

<script>
</script>

<style scoped>

.footer {
    background-color: #1E1E1E;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0px 30px 0px 30px;
    height: 100px;
    position:relative;
    z-index: 2;
}

.footer .logo {
    width: 180px;
}

.buttons {
    display: inline-flex;
    gap: 20px;
    justify-content: space-between;
    height: 40px;
    cursor: pointer;
}

.contact {
    font-family:Sora, sans-serif;
    color: #fff;
    width: auto;
    cursor: pointer;
    text-decoration: none;
    font-weight: normal;
    position: relative;
}

.contact::after {
    content: "";
    position: absolute;
    bottom: 5px;
    left: 0;
    width: 0;
    height: 2px;
    background: #fff;
    transition: all 300ms ease;
}

.contact:hover::after {
    width: 100%;
}

a {
    display:flex;
    justify-content: center;
    align-items: center;
    border-radius: 40px;
    border-style: none;
    cursor: pointer;
}

.icon {
    height: 22px;
    width: 22px;
}

ul {
    padding: 0;
    margin: 0;
}

@media screen and (max-width: 600px) {
    .footer {
        flex-direction: column;
        padding: 15px
    }
}

</style>