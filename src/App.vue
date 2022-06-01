<template>
  <div id="app">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
@import 'styles/styles.css';
@import url('https://unpkg.com/boxicons@2.0.7/css/boxicons.min.css');
/* #app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>
