<template>
  <PageNavbar></PageNavbar>
  <router-view :class="{ 'router': $route.path !== '/' }" />
</template>

<script setup lang="ts">
import PageNavbar from './components/PageNavbar.vue';


</script>

<style lang="scss">

* {
  font-family: Tahoma, Helvetica, Arial, "Microsoft Yahei", STXihei, sans-serif;
}

.router {
  margin-top: 3rem;
}

html,
body,
#app {
  margin: 0;
  padding: 0;
  overflow-x: hidden;
  background-color: #47525e;
  overflow-y: overlay;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #e0e2e9;
}

::-webkit-scrollbar {
  width: 7px;
}

::-webkit-scrollbar-track {
  border-radius: 10px;
  background-color: #a8a8a818;
}

::-webkit-scrollbar-thumb {
  background: rgba(214, 214, 214, 0.377);
  border-radius: 1rem;
}

::-webkit-scrollbar-thumb:hover {
  background: rgba(214, 214, 214, 0.541);
}
</style>
