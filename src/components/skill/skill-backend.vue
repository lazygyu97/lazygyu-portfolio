<template>
  <div class="skill">
    <div class="language">
      <img src="/src/assets/api.png" />
      <h1>Backend</h1>
    </div>
    <div class="skill-list">
      <div class="detail-skill">Spring Boot</div>
      <div class="detail-skill">Spring Security</div>
      <div class="detail-skill">Lombok</div>
      <div class="detail-skill">Redis</div>
      <div class="detail-skill">JPA</div>
      <div class="detail-skill">RestTemplate</div>
      <div class="detail-skill">···</div>
    </div>
  </div>
</template>

<script setup>
import "@/styles/detail-skill.scss"; // CSS 파일을 import
</script>

<style scoped>
.detail-skill:nth-child(1) {
  background-color: #4caf50; /* 초록: Spring Boot */
}

.detail-skill:nth-child(2) {
  background-color: #6bc7eb; /* 파랑: Spring Security */
}

.detail-skill:nth-child(3) {
  background-color: #ff6b6b; /* 빨강: Lombok */
}

.detail-skill:nth-child(4) {
  background-color: #ff7043; /* 오렌지: Redis */
}

.detail-skill:nth-child(5) {
  background-color: #4caf50; /* 진한 초록: JPA */
}

.detail-skill:nth-child(6) {
  background-color: #2196f3; /* 깊은 파랑: RestTemplate */
}

.detail-skill:nth-child(7) {
  background-color: #9e9e9e; /* 회색: 기타 */
}
</style>
