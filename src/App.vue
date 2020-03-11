<template>
  <div id="app">
    <div id="nav">
        <site-header></site-header>
        <site-footer></site-footer>
        <soda></soda>
    </div>
    <router-view />
  </div>
</template>

<script>
import SiteHeader from "@/components/SiteHeader.vue";
import SiteFooter from "@/components/SiteFooter.vue";
import Soda from "@/components/Soda.vue";

export default {
  components: {
    SiteHeader,
    SiteFooter,
    Soda
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
