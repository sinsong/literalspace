<template>
  <div style="overflow-x: hidden;">
    <section class="container">
      <intro />
      <div class="links">
        <a href="https://github.com/sinsong/"
           target="_blank"
           class="button--green"
        >GitHub</a>
        <a href="https://space.bilibili.com/30819561"
           target="_blank"
           class="button--green"
        >Bilibili</a>
      </div>
    </section>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import intro from '~/components/index/intro.vue'

export default {
  components: {
    Logo,
    intro
  }
}
</script>

<style>
.container {
  margin: 0;
  padding: 0;
  min-width: 100vw;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  background-image: url(/photo-by-pasquale-vitiello-n-1201.jpg);
  background-position: center center;
  background-repeat: no-repeat;
}

.links {
  padding-top: 15px;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}
</style>
