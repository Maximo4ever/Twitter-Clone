<script setup>
import TwitterIcon from '../assets/TwitterIcon.vue';
import HomeIcon from '../assets/HomeIcon.vue';
import ExploreIcon from '../assets/ExploreIcon.vue';
import NotificationsIcon from '../assets/NotificationsIcon.vue';
import MessagesIcon from '../assets/MessagesIcon.vue';
import BookmarksIcon from '../assets/BookmarksIcon.vue';
import ListsIcon from '../assets/ListsIcon.vue';
import ProfileIcon from '../assets/ProfileIcon.vue';
import MoreIcon from '../assets/MoreIcon.vue';
</script>
<template>
  <header class="header">
    <div class="header__content">
      <div class="header__logo">
        <TwitterIcon width="33" height="38" />
      </div>
      <ul class="header__menu">
        <li class="active"><HomeIcon width="28" height="28" /> Home</li>
        <li><ExploreIcon width="28" height="28" /> Explore</li>
        <li><NotificationsIcon width="28" height="28" /> Notifications</li>
        <li><MessagesIcon width="28" height="28" /> Messages</li>
        <li><BookmarksIcon width="28" height="28" /> Bookmarks</li>
        <li><ListsIcon width="28" height="28" /> Lists</li>
        <li><ProfileIcon width="28" height="28" /> Profile</li>
        <li><MoreIcon width="28" height="28" /> More</li>
        <button class="header__menu__twittear">Twittear</button>
      </ul>
    </div>
  </header>
</template>
<style>
.header {
  width: 275px;
}
.header__content {
  position: fixed;
}
.header__logo {
  padding: 12px;
}
.header__menu {
  list-style: none;
}
.header__menu li {
  display: flex;
  align-items: center;
  column-gap: 19px;
  font-size: 20px;
  font-weight: 400;
  padding: 12px;
  margin-block: 4px;
  cursor: pointer;
}
.header__menu li:hover {
  background-color: #2C3640;
  border-radius: 26px;
}
.header__menu .active {
  font-weight: 800;
}
.header__menu__twittear {
  width: 225px;
  height: 52px;
  font-size: 17px;
  color: #fff;
  font-weight: 800;
  background-color: #1d9bf0;
  border: none;
  border-radius: 40px;
  margin-top: 16px;
  cursor: pointer;
}
.header__menu__twittear:hover {
  background-color: #1A8CD8;
}
</style>