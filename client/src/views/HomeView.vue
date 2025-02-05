<template>
  <main>
    <description-disclaimer/>
    <conversion-calculator/>
    <calculator-history/>
  </main>
</template>

<script>
import descriptionDisclaimer from '../components/DescriptionDisclamer.vue';
import conversionCalculator from '../components/ConversionCalculator.vue';
import calculatorHistory from '../components/CalculatorHistory.vue';

export default {
  components: {
    descriptionDisclaimer,
    conversionCalculator,
    calculatorHistory,
  }
}
</script>

<style scoped>
main {
  margin: 0 auto;
  margin-top: 3rem;
  text-align: center;
}

.content-box {
  background-color: var(--green);
  border: var(--green-dark) solid 3px;
  border-radius: 8px;
  padding: 1rem;
}
</style>