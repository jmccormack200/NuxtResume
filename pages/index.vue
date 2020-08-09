<template>
  <div id="app" class="container">
    <Header />
    <hr class="line-break" />
    <Experience />
    <hr class="line-break" />
    <Education />
    <hr class="line-break" />
    <Skills />
    <hr class="line-break" />
    <Interests />
  </div>
</template>

<script>
import Header from '../src/components/Header'
import Experience from "../src/components/Experience";
import Education from "../src/components/Education";
import Skills from "../src/components/Skills";
import Interests from "../src/components/Interests";

import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
import { library } from '@fortawesome/fontawesome-svg-core'
import { faLinkedinIn, faGithub, faMedium } from '@fortawesome/free-brands-svg-icons'

library.add(faLinkedinIn, faGithub, faMedium)

export default {
  name: 'App',
  components: {
    Interests,
    Skills,
    Education,
    Experience,
    Header
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  margin-top: 60px;
  margin-bottom: 60px;
}

.line-break {
  margin-top: 24px;
  margin-bottom: 24px;
}
</style>
