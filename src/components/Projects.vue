<template>
  <div>
    <h2 class="mb-5">Selected Projects</h2>
    <div v-for="project in projectData" :key="project.title">
      <div class="d-flex flex-column flex-md-row justify-content-between mb-5">
        <div class="flex-grow-1">
          <h3 class="mb-0">{{ project.title }}</h3>
          <div class="subheading mb-3"><strong>Primary Technology:</strong> {{ project.primaryTech }}</div>
          <p>{{ project.description }}</p>
        </div>
        <div class="flex-shrink-0"><span class="text-primary">{{ project.date }}</span></div>
      </div>
    </div>
  </div>
</template>

<script>
import {projectData} from "@/data/projects";

export default {
  name: "Projects",
  data() {
    return {
      projectData: projectData
    }
  }
}
</script>

<style lang="scss" scoped>
h3 {
  font-weight: 600;
  text-transform: uppercase;
}
</style>