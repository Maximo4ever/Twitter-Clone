<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Aside from './components/Aside.vue';
</script>

<template>
  <Header />
  <Main />
  <Aside />
</template>

<style>
@font-face{
  font-family: "TwitterChirp";
  src: url(./assets/chirp-regular-web.woff);
  font-weight: 400;
}
@font-face{
  font-family: "TwitterChirp";
  src: url(./assets/chirp-bold-web.woff);
  font-weight: 600;
}
@font-face{
  font-family: "TwitterChirp";
  src: url(./assets/chirp-heavy-web.woff);
  font-weight: 800;
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family: "TwitterChirp", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  background-color: #15202B;
  color: #fff;
}
#app {
  display: flex;
  align-items: flex-start;
  justify-content: center;
}
</style>
