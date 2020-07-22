<template>
  <div id="app">
    <div class="bigb">
      <vueView />
    </div>
  </div>
</template>

<script>
import vueView from './components/vueView.vue'

export default {
  name: 'App',
  components: {
    vueView
  }
}
</script>

<style>
#app,
body,
html {
  padding: 0;
  margin: 0;
  width: 100vw;
  height: 100vh;
}
</style>
