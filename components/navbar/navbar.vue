<template>
  <b-navbar :sticky="!nosticky" toggleable="lg" type="dark" variant="literal" fixed="top">
    <!-- Brand -->
    <b-navbar-brand to="/">literalSpace</b-navbar-brand>

    <b-navbar-toggle target="nav_collapse" />

    <b-collapse is-nav id="nav_collapse">
      <b-navbar-nav>
        <b-nav-item v-for="nitem in navItems" :to="nitem.to" :key="nitem.to">{{nitem.text}}</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<style>

.bg-literal {
  background-color: rgba(56, 56, 56, 0.92) !important;
  /*
    blue - rgba(100, 149, 237, 0.92)
    gray - rgba(56, 56, 56, 0.92)
   */
}

</style>

<script>

export default {
  props: {
    nosticky: Boolean
  },
  data(){return{
    navItems: [
      {text: 'PublicKey', to: '/pubkey'}
    ]
  }}
}

</script>
