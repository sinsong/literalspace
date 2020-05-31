<template>
  <section class="container">
    <h1 class="title">Public Key</h1>
    <pre class="info">{{pre_info}}</pre>
    <a href="/public_key.asc" style="display:block;text-align:right;">plain text</a>
    <pre class="pubkey">{{pre_publickey}}</pre>
  </section>
</template>

<style scoped>
.container {
  min-height: 100vh;
  max-width: 600px;
}

.title {
  text-align: center;
  font-size: 50px;
  margin: 20px;
}

.info {
  font-size:16px;
  font-family: Consolas, monospace;
}

.pubkey {
  font-size: 16px;
  line-height: 1em;
  font-family: Consolas, monospace;
  word-break: keep-all;
  overflow: hidden;
}
</style>

<script>
const info = `literal kernel
E-mail: 714554019@qq.com
Finger print:
    ACDF E70C 98F4 2F62 0103  BBAF 9550 49A1 EB1C 9A70` ;

import public_key from '~/static/public_key.asc'

export default {
  data() {
    return {
      'pre_info':info,
      'pre_publickey': public_key
    }
  }
}
</script>
