<template>
  <div>
    <h2 class="mb-5">Colleague Feedback</h2>
    <p><em>All feedback below was provided by my colleagues. It has only been altered to redact client names.</em></p>
  <div v-for="feedback in feedbackData" :key="feedback.author">
      <div class="d-flex flex-column flex-md-row justify-content-between mb-5">
        <div class="flex-grow-1">
          <h4 class="mb-0">From: {{ feedback.author }}</h4>
          <br />
          <p>{{ feedback.feedback }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import {feedbackData} from "@/data/feedback";

export default {
  name: "Feedback.vue",
  data() {
    return {
      feedbackData: feedbackData
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