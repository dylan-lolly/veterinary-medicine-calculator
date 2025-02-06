<template>
  <div class="content-box">
    <form v-on:submit.prevent="calcualte">
      <h2>Conversion Calculator</h2>
      <div id="fields">
        <div class="field">
          <label for="patientWeight">Patient Weight</label>
          <input type="text"
          id="patientWeight"
          placeholder="patient weight"
          required
          />
        </div>
        <div class="field">
          <label for="mgPerKg">mg/kg</label>
          <input type="text"
          id="mgPerKg"
          placeholder="mg/kg"
          required
          />
        </div>
        <div class="field">
          <label for="mgStrength">mg Strength</label>
          <input type="text" 
          id="mgStrength"
          placeholder="mg strength"
          required
          />
        </div>
        <div class="field">
          <label for="isLiquid">Liquid Medication</label>
          <input type="checkbox" 
          id="isLiquid"
          />
        </div>
        <div class="field" :class="{'hidden': !isLiquid}">
          <label for="mgPerMl">mg/mL</label>
          <input type="text"
          id="mgPerMl"
          placeholder="mg/mL"
          />
        </div>
      </div>
    </form>
  </div>
</template>

<script>

</script>

<style scoped>
.content-box {
    margin-bottom: 1.5rem;
}

h2 {
    margin-bottom: 1rem;
}

#fields {
    display: flex;
    justify-content: space-around;
}

.field {
    display: flex;
    flex-direction: column-reverse;
    align-items: center;
}

input[type=text] {
  border: 1px solid #dbdbdb;
  border-radius: 4px;
  color: #323539;
  height:35px;
  padding: 0 .5rem;
  width: 100px;
}

label {
    font-size: 1.2rem;
}
</style>