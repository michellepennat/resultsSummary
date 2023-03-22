<template>
  <section class="summary">
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
