<template>
  <div id="app">
    <div id="app" :class="typeof weather.main != 'undefined' && weather.main.temp > 16 ? 'warm' : ''">
    <main>
      <div class="search-box">
        <input 
          type="text" 
          class="search-bar" 
          placeholder="Search..."
          v-model="query"
          @keypress="fetchWeather"
        />
      </div>
    
  </div>
</template>

<script>


export default {
  name: 'App',
 
}
</script>

<style>

</style>
