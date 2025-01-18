<template>
  <div style="background-color: #f3cd50">
    <div class="custom-container">
      <div style="margin-bottom: 50px"><h1>SKILL</h1></div>
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
  background-color: #f3cd50;
  /* Flexbox 설정 */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  height: 50vh;
}

.introduce-layer {
  display: flex;
  width: 100%; /* 전체 너비를 100%로 설정 */
  height: 150px;
}

.skill-layer {
  /* Rectangle 19 */
  width: 80%;
  height: 70%;

  background: #fffde7;
  border-radius: 20px;

  /* Flexbox 설정 */
  display: flex;
  flex-direction: column; /* 요소를 수직으로 정렬 */
  justify-content: space-evenly; /* 요소 간 간격을 동일하게 */
  align-items: center; /* 수평 중앙 정렬 */
  text-align: center;
}
</style>
