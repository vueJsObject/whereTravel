<template>
  <div>
    <city-header></city-header>
    <city-search></city-search>
    <city-list></city-list>
  </div>
</template>
<script>
import CityHeader from './components/Header'
import CitySearch from './components/Search'
import cityList from './components/List'
export default {
  name: 'City',
  components: {
    CityHeader,
    CitySearch,
    cityList
  }
}
</script>
<style lang="stylus" scoped>
</style>
