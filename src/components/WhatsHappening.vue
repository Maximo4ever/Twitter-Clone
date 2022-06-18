<template>
  <form class="whatsHappening">
    <img class="whatsHappening__img" src="https://thispersondoesnotexist.com/image" alt="random"/>
    <div>
      <input class="whatsHappening__input" type="text" placeholder="What's happening?">
      <div class="whatsHappening__submitContainer">
        <div></div>
        <button class="whatsHappening__btn" type="submit">Twittear</button>
      </div>
    </div>
  </form>
</template>
<style>
.whatsHappening {
  display: flex;
  align-items: flex-start;
  padding-inline: 16px;
  padding-block: 10px;
  border-bottom: 1px solid #38444d;
}
.whatsHappening__img {
  width: 52px;
  height: 52px;
  border-radius: 50%;
  object-fit: cover;
  margin-right: 12px;
}
.whatsHappening__input {
  font-size: 20px;
  color: #f7f9f9;
  background-color: transparent;
  border: none;
  outline: none;
  padding-block: 12px;
}
.whatsHappening div {
  width: 100%;
}
.whatsHappening__submitContainer {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.whatsHappening__btn {
  font-size: 15px;
  font-weight: 700;
  padding: 10px 20px;
  color: #fff;
  background-color: #1d9bf0;
  border: none;
  border-radius: 20px;
}
</style>