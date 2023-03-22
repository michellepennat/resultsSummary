<template>
  <main class="result-summary" role="main">
    <div class="content">
      <ResultComponent />
      <SummaryComponent />
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
