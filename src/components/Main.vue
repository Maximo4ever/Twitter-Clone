<script setup>
import Nav from "./Nav.vue";
import WhatsHappening from "./WhatsHappening.vue";
import Tweet from "./Tweet.vue";
</script>
<template>
  <main class="main">
    <Nav />
    <WhatsHappening />
    <Tweet />
    <Tweet />
    <Tweet />
    <Tweet />
    <Tweet />
    <Tweet />
    <Tweet />
  </main>
</template>
<style>
.main {
  width: 600px;
  border-inline: 1px solid #38444d;
}
</style>