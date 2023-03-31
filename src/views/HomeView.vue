<template>
  <div class="home">
    <Header id="header"/>
    <Intro id="introduction"/>
    <Resume id="resume"/>
    <Projects id="projects"/>
    <ButtonTop/>
    <Footer/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Intro from '@/components/Intro.vue'
import Resume from '@/components/Resume.vue'
import Projects from '@/components/Projects.vue'
import ButtonTop from '@/components/ButtonTop.vue'
import Footer from '@/components/Footer.vue'


export default {
  name: 'HomeView',
  components: {
    Header,
    Intro,
    Resume,
    Projects,
    ButtonTop,
    Footer
  }
}
</script>

<style>

.home {
  margin: 0;
  padding: 0;
}

</style>