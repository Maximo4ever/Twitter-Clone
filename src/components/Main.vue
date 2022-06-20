<script setup>
import Nav from "./Nav.vue";
import WhatsHappening from "./WhatsHappening.vue";
import Tweet from "./Tweet.vue";

const people = Array.from({length:20})
</script>
<template>
  <main class="main">
    <Nav />
    <WhatsHappening />
    <div v-for="(n,index) in people">
      <Tweet :index="index" />
    </div>
  </main>
</template>
<style>
.main {
  width: 600px;
  border-inline: 1px solid #38444d;
}
</style>