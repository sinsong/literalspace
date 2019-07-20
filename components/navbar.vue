<template>
  <b-navbar toggleable="lg" type="dark" :sticky="index?false:true" variant="literal" fixed="top">
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

<script>
import { page_info } from '~/common/pages'

export default {
  data(){return{
    navItems: page_info
  }},
  props:{
    index: Boolean
  }
}
</script>
