<template>
  <div class="leading-normal tracking-normal text-white gradient">
    <the-header />
    <nuxt />
    <the-footer />
    <script src="/__/firebase/7.14.2/firebase-app.js"></script>
    <script src="/__/firebase/7.14.2/firebase-analytics.js"></script>
    <script src="/__/firebase/init.js"></script>
  </div>
</template>

<script>
import TheHeader from '@/components/TheHeader.vue'
import TheFooter from '@/components/TheFooter.vue'

export default {
  components: {
    'the-header': TheHeader,
    'the-footer': TheFooter
  }
}
</script>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

.gradient {
  /* background: linear-gradient(90deg, #6200ee 0%, #03dac5 100%);  */
  background: linear-gradient(90deg, #2196f3 0%, #3f51b5 100%);
}
</style>
