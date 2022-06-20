<script setup>
import CommentIcon from "../assets/CommentIcon.vue";
import RetweetIcon from "../assets/RetweetIcon.vue";
import LikeIcon from "../assets/LikeIcon.vue";
import ShareIcon from "../assets/ShareIcon.vue";
import Options from "../assets/Options.vue";
defineProps({
  index: Number
})
</script>
<template>
  <article class="tweet">
    <img class="tweet__img" :src="`https://xsgames.co/randomusers/assets/avatars/male/${index}.jpg`" alt="random"/>
    <div class="tweet__body">
      <header class="tweet__body__header">
        <div class="tweet__body__header__content">
          <h6 class="tweet__body__name">John Doe</h6><span>@elonmusk</span> <span>· 13h</span>
        </div>
        <Options />
      </header>
      <p class="tweet__body__text">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Dolores, libero! Velit ipsa eos distinctio vitae. Nam autem tenetur ab, in adipisci atque amet architecto facilis exercitationem, reiciendis libero a sequi. Lorem ipsum dolor sit amet consectetur adipisicing elit. Vel?</p>
      <div class="tweet__body__social">
        <div style="--hBg:#1C3345;--hColor:#1D9BF0;">
          <span class="tweet__body__social__icon">
            <CommentIcon />
          </span>
          <span class="tweet__body__social__num">129</span>
        </div>
        <div style="--hBg:#19363A;--hColor:#00BA7C">
          <span class="tweet__body__social__icon">
            <RetweetIcon />
          </span>
          <span class="tweet__body__social__num">831</span>
        </div>
        <div style="--hBg:#32253A;--hColor:#F91880">
          <span class="tweet__body__social__icon">
            <LikeIcon />
          </span>
          <span class="tweet__body__social__num">1214</span>
        </div>
        <div style="--hBg:#1C3345;--hColor:#1D9BF0">
          <span class="tweet__body__social__icon">
            <ShareIcon />
          </span>
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
  padding-block: 12px 7px;
  border-bottom: 1px solid #38444d;
  cursor: pointer;
}
.tweet:hover {
  background-color: #1C2732;
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
.tweet__body__name:hover {
  text-decoration: underline;
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
  margin-top: 2px;
  margin-left: -8px;
  color: #8b98a5;
}
.tweet__body__social div {
  display: flex;
  align-items: center;
  cursor: pointer;
}
.tweet__body__social div:hover .tweet__body__social__icon {
  background-color: var(--hBg);
}
.tweet__body__social div:hover .tweet__body__social__num {
  color: var(--hColor);
}
.tweet__body__social__icon {
  display: flex;
  align-items: center;
  padding: 8px;
  border-radius: 50%;
}
.tweet__body__social__num {
  padding-inline: 6px;
}
</style>