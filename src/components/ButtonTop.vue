<template>
    <div class="button-top">
        <a href="#" v-scroll-to="'#header'"><img src="@/assets/arrow_top.png" alt="Retour en haut de page" class="arrow-top" /></a>
    </div>  
</template>

<script>
</script>

<style scoped>

.button-top {
    display: flex;
    position: fixed;
    bottom: 50px;
    right: 50px;
    z-index: 1;
}

a {
    display: flex;
    background-color: #1E1E1E;
    border-radius: 40px;
    padding: 10px;
    border-style: none;
    width: 45px;
    height: 45px;
    cursor: pointer;
    justify-content: center;
    align-items: center;
}

.arrow-top {
    height: 90%;
}

</style>