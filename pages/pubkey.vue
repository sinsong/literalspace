<template>
  <section class="container">
    <h1 class="title">Public Key</h1>
    <pre style="font-size: 20px">E-mail: 714554019@qq.com</pre>
    <pre style="font-size: 20px">Finger print:</pre>
    <pre style="font-size: 16px">E010 C4C9 B2EA E272 EF15  0DDD 3099 D4BB 7E40 0971</pre>
    <a href="/public_key.asc" style="padding: 10px;">plain text</a>
    <pre class="pubkey">{{publickey}}</pre>
  </section>
</template>

<style>
.container {
  min-height: 100vh;
  max-width: 600px;

  text-align: center;

  margin-top: 70px;
}

.title {
  font-size: 50px;
  margin: 10px;
}

.pubkey {
  text-align: left;
  font-size: 16px;
  line-height: 1em;
  font-family: Consolas, monospace;
  word-break: keep-all;
  overflow: hidden;
}
</style>

<script>
const pub_key = 
      ['-----BEGIN PGP PUBLIC KEY BLOCK-----',
        '',
        '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',
        '=vYzm',
        '-----END PGP PUBLIC KEY BLOCK-----'
      ].join('\n');

export default {
  data() {
    return {
      'publickey': pub_key
    }
  }
}
</script>
