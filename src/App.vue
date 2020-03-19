<template>
  <div id="app">
    <headernav />
    <router-view />
  </div>
</template>
<script>
import headernav from "./components/headernav";
export default {
  components: {
    headernav
  },
  mounted() {
  }
};
</script>

<style>
</style>
