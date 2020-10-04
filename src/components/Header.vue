<template>
  <div>
    <h1 class="mb-0">
      JD
      <span class="header-accent">McCormack</span>
    </h1>
    <div class="subheading text-secondary mb-5">
      Boston, MA - (617) 257-5586 -
      <a href="mailto:me@jdmccormack.com">me@jdmccormack.com</a>
    </div>
    <p class="lead mb-5">I am a passionate and curious software engineer. I am comfortable working across a number of
      tech stacks and am always interested in learning new ones. Despite being a "switch hitter", I strive to learn best practices
      for each platform. I see new languages as "tools in a toolbox" and work to understand the benefits and pitfalls
      of each.</p>

    <p class="lead mb-5">I float comfortably between being a "hands on keyboard" developer, and a team lead. I enjoy
    putting processes in place when needed, but also pulling them out when they're hindering progress. I like to focus on
    the individuals in a team to find better ways to unblock them and allow them to achieve at their highest level. </p>
    <div class="social-icons">
      <a class="social-icon" href="https://www.linkedin.com/in/jdmccormack/">
        <font-awesome-icon :icon="['fab', 'linkedin-in']"/>
      </a>
      <a class="social-icon" href="https://github.com/jmccormack200">
        <font-awesome-icon :icon="['fab', 'github']"/>
      </a>
      <a class="social-icon" href="https://medium.com/@jdmccormack63">
        <font-awesome-icon :icon="['fab', 'medium']"/>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style lang="scss" scoped>
@import "src/assets/scss/colors.scss";

.social-icons {
  display: flex;
  width: 100%;
  justify-content: left;
}

.social-icon {
  display: inline-flex;
  align-items: center;
  height: 3.5rem;
  width: 3.5rem;
  justify-content: center;
  background-color: $color-primary;
  color: #fff;
  border-radius: 100%;
  font-size: 1.5rem;
  margin-right: 1.5rem;
}

.social-icon:hover {
  background-color: $color-accent
}
</style>