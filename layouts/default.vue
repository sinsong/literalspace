<template>
  <div>
    <navbar />
    <nuxt />
    <footer style="text-align:center">
      <p>©2019 literal kernel, powered by <b-link href="https://nuxtjs.org" target="_blank">Nuxt.js</b-link></p>
      <p>Made with ❤ by literal kernel</p>
    </footer>
  </div>
</template>

<style>
html {
  font-family: Consolas, 'Microsoft YaHei', 'Helvetica Neue', sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.bg-literal {
  background-color: rgba(56, 56, 56, 0.92) !important;
  /*
    blue - rgba(100, 149, 237, 0.92)
    gray - rgba(56, 56, 56, 0.92)
   */
}

.nuxt-link-active, .route-link-active{
  color: #fff !important;
  font-weight: 6000 !important;
}

</style>

<script>
import navbar from '~/components/navbar.vue'

export default {
  components:{
    navbar
  }
}
</script>
