<template>
  <div class="home">
    <Header id="header"/>
    <div class="container">
      <Intro id="introduction"/>
      <About id="about"/>
      <Projects id="projects"/>
    </div>
    <ButtonTop/>
    <Footer/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Intro from '@/components/Intro.vue'
import About from '@/components/About.vue'
import Projects from '@/components/Projects.vue'
import ButtonTop from '@/components/ButtonTop.vue'
import Footer from '@/components/Footer.vue'


export default {
  name: 'HomeView',
  components: {
    Header,
    Intro,
    About,
    Projects,
    ButtonTop,
    Footer
  }
}
</script>

<style>

.home {
  margin: 0 auto;
  padding: 0;
}

.container {
  padding: 0 50px;
  max-width: 1264px;
  margin: auto;
}

@media screen and (max-width: 800px) {
  .container {
    padding: 0 30px;
  }
}

</style>