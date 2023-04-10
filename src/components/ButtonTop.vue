<template>
    <div class="button-top">
        <a href="#" v-scroll-to="'#header'"><img src="@/assets/arrow_top.png" alt="Retour en haut de page" class="arrow-top" /></a>
    </div>  
</template>

<script>
</script>

<style scoped lang="scss">

.button-top {
    display: flex;
    position: fixed;
    bottom: 50px;
    right: 50px;
    z-index: 1;

    &:hover {
        .arrow-top {
            animation: 1s ease 1 arrow;
        }
    }
}

@keyframes arrow {
    50% { transform:translateY(-200%); }
    51% { transform:translateY(100%); }
    100% { transform:translateY(0%); }
 }

a {
    display: flex;
    background-color: var(--colors-black);
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