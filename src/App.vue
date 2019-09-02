<template>
  <div id="app">
    <div class="container">
      <Header />
      <router-view />
    </div>
  </div>
</template>

<script>
import Header from './components/Header';
export default {
  name: 'App',
  components: {
    Header
  }
};
</script>

<style>
body {
  padding: 30px
}
</style>
