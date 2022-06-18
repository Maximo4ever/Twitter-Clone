<script setup>
import CommentIcon from "../assets/CommentIcon.vue";
import RetweetIcon from "../assets/RetweetIcon.vue";
import LikeIcon from "../assets/LikeIcon.vue";
import ShareIcon from "../assets/ShareIcon.vue";
import Options from "../assets/Options.vue";
</script>
<template>
  <article class="tweet">
    <img class="tweet__img" src="https://thispersondoesnotexist.com/image" alt="random"/>
    <div class="tweet__body">
      <header class="tweet__body__header">
        <div class="tweet__body__header__content">
          <h6 class="tweet__body__name">John Doe</h6><span>@elonmusk</span> <span>· 13h</span>
        </div>
        <Options />
      </header>
      <p class="tweet__body__text">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Dolores, libero! Velit ipsa eos distinctio vitae. Nam autem tenetur ab, in adipisci atque amet architecto facilis exercitationem, reiciendis libero a sequi.</p>
      <div class="tweet__body__social">
        <div>
          <CommentIcon hoverColor="" />
          <span>129</span>
        </div>
        <div>
          <RetweetIcon hoverColor="" />
          <span>831</span>
        </div>
        <div>
          <LikeIcon hoverColor="" />
          <span>1214</span>
        </div>
        <div>
          <ShareIcon hoverColor="" />
        </div>
      </div>
    </div>
  </article>
</template>
<style> 
.tweet {
  display: flex;
  align-items: flex-start;
  padding-inline: 16px;
  padding-block: 12px;
  border-bottom: 1px solid #38444d;
}
.tweet__img {
  width: 52px;
  height: 52px;
  border-radius: 50%;
  object-fit: cover;
  margin-right: 12px;
}
.tweet__body__header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 4px;
}
.tweet__body__header__content {
  display: flex;
  align-items: center;
  gap: 5px;
  color: #8b98a5;
}
.tweet__body__name {
  font-size: 15px;
  font-weight: 800;
  color: #fff;
}
.tweet__body__text {
  font-size: 15px;
  line-height: 20px;
  font-weight: 400;
}
.tweet__body__social {
  width: 100%;
  max-width: 425px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  font-size: 13px;
  margin-block: 12px 1px;
  color: #8b98a5;
}
.tweet__body__social div {
  display: flex;
  align-items: center;
  cursor: pointer;
}
.tweet__body__social span {
  padding-inline: 12px;
}
</style>