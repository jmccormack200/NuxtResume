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
import Header from './components/Header'
import Experience from "@/components/Experience";
import Education from "@/components/Education";
import Skills from "@/components/Skills";
import Interests from "@/components/Interests";

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
