<template>
  <b-navbar toggleable="lg" type="dark" variant="literal" fixed="top">
    <!-- Brand -->
    <b-navbar-brand href="/">literalSpace</b-navbar-brand>

    <b-navbar-toggle target="nav_collapse" />

    <b-collapse is-nav id="nav_collapse">
      <b-navbar-nav>
        <b-nav-item href="/pubkey">PublicKey</b-nav-item>
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
