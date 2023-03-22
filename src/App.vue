<template>
  <main>
    <ResultComponent />
    <SummaryComponent />
    <div class="attribution">
      Challenge by
      <a
        href="https://www.frontendmentor.io/challenges/results-summary-component-CE_K6s0maV"
        target="_blank"
        >Frontend Mentor</a
      >. Coded by
      <a href="https://github.com/michellepennat">Michelle Penna</a>.
    </div>
  </main>
</template>

<script>
import ResultComponent from "./components/result/result.vue";
import SummaryComponent from "./components/summary/summary.vue";
export default {
  name: "App",
  components: { ResultComponent, SummaryComponent },
};
</script>
