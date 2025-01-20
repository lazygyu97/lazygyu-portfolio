<template>
  <div class="top-container">
    <div class="custom-container">
      <div><h1>SKILL</h1></div>
      <div class="skill-layer">
        <language />
        <backend />
        <database />
        <frontend />
        <devOps />
      </div>
    </div>
  </div>
</template>

<script setup>
import Language from "@/components/skill/skill-language.vue";
import Frontend from "@/components/skill/skill-frontend.vue";
import Backend from "@/components/skill/skill-backend.vue";
import Database from "@/components/skill/skill-database.vue";
import DevOps from "@/components/skill/skill-devOps.vue";
</script>

<style scoped>
.custom-container {
  margin: 0 auto;
  padding: 0 20px;
  max-width: 1550px;
  /* Flexbox 설정 */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  height: 50vh;
}
.top-container {
  width: 100%;
  background-color: #f3cd50;
}
.skill-layer {
  width: 70%;
  height: 60%;
  background: #fffde7;
  border-radius: 20px;
  /* Flexbox 설정 */
  display: flex;
  flex-direction: column; /* 요소를 수직으로 정렬 */
  justify-content: space-evenly; /* 요소 간 간격을 동일하게 */
  align-items: center; /* 수평 중앙 정렬 */
  text-align: center;
  margin-top: 30px;
}
@media (max-width: 1440px) {
  .skill-layer {
    width: 95%; /* 작은 화면에서는 더 넓게 */
    margin-top: 20px; /* 요소 간 여백 줄이기 */
  }
}
/* 화면 크기가 768px 이하일 때의 스타일 */
@media (max-width: 768px) {
  .custom-container {
    height: auto;
    padding: 30px 10px; /* 모바일 화면에서는 좌우 여백을 줄임 */
  }
  .skill-layer {
    width: 90%; /* 작은 화면에서는 더 넓게 */
    height: auto;
    margin-top: 20px; /* 요소 간 여백 줄이기 */
    padding-top: 30px;
    padding-bottom: 30px;
  }
  .skill-layer > * {
    margin-bottom: 15px; /* 각 컴포넌트 간의 간격을 더 좁힘 */
  }
}

/* 화면 크기가 480px 이하일 때의 스타일 */
@media (max-width: 480px) {
  .custom-container {
    height: auto;
  }

  .skill-layer {
    width: 98%; /* 화면에 맞게 너비 설정 */
    height: auto;
    margin-top: 20px;
    padding-top: 30px;
    padding-bottom: 30px;
  }

  .skill-layer > * {
    margin-bottom: 50px; /* 모바일에서는 각 컴포넌트 간 간격을 더 좁힘 */
  }
}
</style>
