<template>
  <div class="skill">
    <div class="language">
      <img src="/src/assets/devops.png" />
      <h1>DevOps</h1>
    </div>
    <div class="skill-list">
      <div class="detail-skill">AWS</div>
      <div class="detail-skill">Git</div>
      <div class="detail-skill">GitHub Actions</div>
      <div class="detail-skill">Linux</div>

      <div class="detail-skill">···</div>
    </div>
  </div>
</template>

<script setup>
import "@/styles/detail-skill.scss"; // CSS 파일을 import
</script>

<style scoped>
.detail-skill:nth-child(1) {
  background-color: #00acc1; /* 청록색 */
}

.detail-skill:nth-child(2) {
  background-color: #e91e63; /* 핑크 */
}

.detail-skill:nth-child(3) {
  background-color: #9c27b0; /* 보라색 */
}

.detail-skill:nth-child(4) {
  background-color: #4caf50; /* 초록색 */
}
.detail-skill:nth-child(5) {
  background-color: #9e9e9e; /* 회색 */
}
</style>
