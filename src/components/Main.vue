<script setup>
import Nav from "./Nav.vue";
import WhatsHappening from "./WhatsHappening.vue";
import Tweet from "./Tweet.vue";

const people = Array.from({length:20});
const tweets = [
  {
    type: "onlyText",
    src: "none"
  },
  {
    type: "image",
    src: "/images/tweetImg.jpg"
  },
  {
    type: "image",
    src: "/images/tweetImg2.jpg"
  },
  {
    type: "groupImages",
    src: ["/images/tweetImg3.jpg","/images/tweetImg5.jpg","/images/tweetImg6.jpg","/images/tweetImg7.jpg"]
  },
  {
    type: "image",
    src: "/images/tweetGif.gif"
  }
];
</script>
<template>
  <main class="main">
    <Nav />
    <WhatsHappening />
    <Tweet v-for="(tweet,index) in tweets" :index="index" :tweet="tweet" />
  </main>
</template>
<style>
.main {
  width: 600px;
  border-inline: 1px solid #38444d;
}
</style>