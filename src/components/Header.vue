<template>
  <div>
    <h1 class="mb-0">
      JD
      <span class="header-accent">McCormack</span>
    </h1>
    <div class="subheading text-secondary mb-5">
      Boston, MA · (617) 257-5586 ·
      <a href="mailto:me@jdmccormack.com">me@jdmccormack.com</a>
    </div>
    <p class="lead mb-5">I am experienced in leveraging agile frameworks to provide a robust synopsis for high level
      overviews. Iterative approaches to corporate strategy foster collaborative thinking to further the overall value
      proposition.</p>
    <div class="social-icons">
      <a class="social-icon" href="#">
        <font-awesome-icon :icon="['fab', 'linkedin-in']"/>
      </a>
      <a class="social-icon" href="#">
        <font-awesome-icon :icon="['fab', 'github']"/>
      </a>
      <a class="social-icon" href="#">
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

h1 {
  font-size: 6rem;
  text-transform: uppercase;
  color: $color-primary;
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