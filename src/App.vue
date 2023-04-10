<template>
  <router-view />
</template>

<style lang="scss">

:root {
  --colors-black: #1e1e1e;
  --colors-blue: #11b2cc;
  --colors-grey: #c4c4c4;
  --container-width: 1264px;
}

* {
  box-sizing: border-box;
}

#app {
  font-family: Sora, sans-serif;
  background-color: #ffff;
  color: var(--colors-black);
}

body {
  margin: 0;
}

.button {
    display: flex;
    background-color: var(--colors-black);
    border-radius: 40px;
    font-family: Sora, sans-serif;
    font-size: 15px;
    color: #fff;
    padding: 10px;
    border-style: solid;
    border-color: var(--colors-black);
    border-width: 1px;
    text-decoration: none;
    width: auto;
    cursor: pointer;
    text-align: left;
    overflow: hidden;
    transition: 0.2s transform ease-in-out;
    will-change: transform;
    z-index: 0;

    &::after {
      background-color: #fff;
      border-radius: 40px;
      content: '';
      display: block;
      height: 100%;
      width: 100%;
      position: absolute;
      left: 0;
      top: 0;
      transform: translate(-100%, 0) rotate(10deg);
      transform-origin: top left;
      transition: 0.2s transform ease-out;
      will-change: transform;
      z-index: -1;
    }

    &:hover {
      border: 1px solid var(--colors-black);
      color: var(--colors-black);
      will-change: transform;
      
      &::after {
        transform: translate(0, 0);
      }
    }
}

.box {
  background-color: #fff;
  border-radius:12px;
  border-style: solid;
  border-width: 1px;
  border-color: var(--colors-black);
  margin: 0 0 50px 0;
  box-shadow: 4px 4px 0px var(--colors-black);
}

@media screen and (max-width: 800px) {
  .button {
    font-family:Sora, sans-serif;
    font-size: 13px;
  }
}

</style>
