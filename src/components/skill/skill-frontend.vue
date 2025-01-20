<template>
  <div class="skill">
    <div class="language">
      <img src="/src/assets/html.png" />
      <h1>Frontend</h1>
    </div>
    <div class="skill-list">
      <div class="detail-skill">HTML</div>
      <div class="detail-skill">CSS</div>
      <div class="detail-skill">JS</div>
      <div class="detail-skill">Vue.js</div>
      <div class="detail-skill">Axios</div>
      <div class="detail-skill">···</div>
    </div>
  </div>
</template>

<script setup>
import "@/styles/detail-skill.scss"; // CSS 파일을 import
</script>

<style scoped>
.detail-skill:nth-child(1) {
  background-color: #f44336; /* 빨강 */
}

.detail-skill:nth-child(2) {
  background-color: #2196f3; /* 파랑 */
}

.detail-skill:nth-child(3) {
  background-color: #4caf50; /* 초록 */
}

.detail-skill:nth-child(4) {
  background-color: #ff5722; /* 오렌지 */
}

.detail-skill:nth-child(5) {
  background-color: #009688; /* 청록색 */
}

.detail-skill:nth-child(6) {
  background-color: #9e9e9e; /* 회색 */
}
</style>
