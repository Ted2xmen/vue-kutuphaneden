<template>
  <div id="navApp">
      <TheNav/>
      <router-view/>
  </div>

</template>

<style>

a {
  font-weight: bold;
  color: #a0abb6  !important;
}

 a.router-link-exact-active {
  color: #42b983 !important;
}
</style>

<script>
// @ is an alias to /src
import TheNav from '@/components/TheNav.vue'
export default {
  name: 'Home',
  components: {
    TheNav
  }
}
</script>
