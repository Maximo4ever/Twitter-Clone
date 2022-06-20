<script setup>
import SearchIcon from "../assets/SearchIcon.vue";
import AsideUser from "./AsideUser.vue";
const usersToFollow = Array.from({length:4})
</script>
<template>
  <aside class="aside">
    <div class="aside__content">
      <form class="form">
        <SearchIcon width="20px" height="20px" />
        <input class="form__input" type="text" placeholder="Search Twitter">
      </form>
      <section class="section">
        <h3>What’s happening</h3>
      </section>
      <section class="section">
        <h3>Who to follow</h3>
        <div class="userWhoToFollow" v-for="(n,index) in usersToFollow">
          <AsideUser :index="index" />
        </div>
      </section>
    </div>
  </aside>
</template>
<style>
.aside {
  width: 350px;
  height: 100%;
  margin-left: 30px;
  /* background-color: #252E38; */
}
.aside__content {
  width: 350px;
  position: fixed;
  top: 0;
}
.form {
  position: relative;
  padding-top: 12px;
}
.form__input {
  width: 100%;
  font-size: 15px;
  padding: 14px 10px 14px 55px;
  background-color: #273340;
  color: #fff;
  border-radius: 30px;
  border: none;
  outline: none;
}
.form__input::placeholder {
  color: #8B98A5;
}
.section {
  background-color: #1E2732;
  padding-block: 12px;
  border-radius: 16px;
  margin-top: 16px;
}
.section h3 {
  padding-inline: 16px;
}
.userWhoToFollow {
  padding-top: 10px;
}
</style>