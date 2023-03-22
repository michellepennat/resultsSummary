<template>
  <section class="summary" role="document">
    <h4>Summary</h4>
    <ul class="summary__list">
      <li v-for="aspect in aspects" :key="aspect.id">
        <div class="summary__title">
          <img :src="aspect.icon" :alt="aspect.nameAspect" />
          <h5 :class="`title  title--${aspect.color}`">
            {{ aspect.nameAspect }}
          </h5>
        </div>
        <p>{{ aspect.score }} <span>/ 100</span></p>
      </li>
    </ul>
    <button>Continue</button>
    <div class="attribution">
      Challenge by
      <a
        href="https://www.frontendmentor.io/challenges/results-summary-component-CE_K6s0maV"
        target="_blank"
        >Frontend Mentor</a
      >. Coded by
      <a href="https://github.com/michellepennat">Michelle Penna</a>.
    </div>
  </section>
</template>

<script>
import data from "../../data/summary";
export default {
  name: "SummaryComponent",
  data() {
    return {
      aspects: data,
    };
  },
};
</script>
