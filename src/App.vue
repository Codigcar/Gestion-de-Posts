<template>
  <div class="container">
    <app-header/>
    <app-posts/>
    <app-footer/>
  </div>
</template>

<script>

import AppPosts from "@/components/Posts";
import AppHeader from "@/components/Header";
import AppFooter from "@/components/Footer";

export default {
  name: 'App',
  components: {
    AppPosts,
    AppHeader,
    AppFooter
  }
}
</script>

<style>
  @import "../node_modules/bootstrap/dist/css/bootstrap.min.css";
</style>
