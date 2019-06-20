<template lang="html">
  <div v-if="country">
    <h3>{{country.name}}</h3>
    <p>Capital: {{country.capital}}</p>
    <p>Population: {{country.population}}</p>
    <p>Languages: {{country.languages[0].name}}</p>
    <!-- <p>currency: {{country.currencirs[0].name}}</p> -->
    <img class="flag" :src="country.flag" />

  </div>

</template>

<script>
export default {
  name: 'country-detail',
  props: ['country']
}
</script>

<style lang="css" scoped>
.flag {
  height: 250px
}
</style>
