<template>
  <div class="user">
    <img class="user__img" src="https://thispersondoesnotexist.com/image" alt="random">
    <div>
      <div>
        <h6 class="user__name">Jhon Doe</h6>
        <span class="user__at">@elonmusk</span>
      </div>
      <button class="user__btn">Follow</button>
    </div>
  </div>
</template>
<style>
.user {
  display: flex;
  align-items: center;
  column-gap: 12px;
  padding-block: 11px;
  padding-inline: 16px;
  cursor: pointer;
}
.user:hover {
  background-color: #252E38;
}
.user__img {
  height: 52px;
  width: 52px;
  border-radius: 50%;
}
.user > div {
  width: 100%;
  display: flex;
  justify-content: space-between;
}
.user h6, .user span {
  font-size: 15px;
}
.user__name:hover {
  text-decoration: underline;
}
.user span {
  color: #8b98a5;
}
.user__btn {
  font-size: 14px;
  height: 32px;
  font-weight: 600;
  padding-inline: 19px;
  border: none;
  border-radius: 16px;
  cursor: pointer;
}
.user__btn:hover {
  background-color: #D7DBDC;
}
</style>