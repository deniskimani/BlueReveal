<template>
  <div id="app">
    <header-app/>
    <router-view/>
    <footer-app/>
  </div>
</template>
<script>
import HeaderApp from "@/components/Header";
import FooterApp from "@/components/Footer";
export default {
  components: {
    HeaderApp,
    FooterApp
  }
};
</script>
<style>

</style>
