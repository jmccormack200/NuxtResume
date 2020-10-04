<template>
  <div id="app" class="container">
    <Header />
    <hr class="line-break" />
    <Experience />
    <hr class="line-break" />
    <Projects />
    <hr class="line-break" />
    <Education />
    <hr class="line-break" />
    <Skills />
    <hr class="line-break" />
    <Feedback />
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
import Projects from "@/components/Projects";
import Feedback from "@/components/Feedback";

export default {
  name: 'App',
  components: {
    Feedback,
    Projects,
    Interests,
    Skills,
    Education,
    Experience,
    Header
  }
}
</script>

<style lang="scss">
@import "assets/scss/colors.scss";

h1 {
  font-size: 6rem;
  text-transform: uppercase;
  color: $color-primary;
}

h2 {
  color: $color-accent;
}

.header-accent {
  color: $color-accent;
}

a {
  color: $color-accent;
}

.subheading {
  text-transform: uppercase;
  color: $color-secondary;
}

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
