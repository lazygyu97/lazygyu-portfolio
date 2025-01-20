<template>
  <div class="skill">
    <div class="language">
      <img src="/src/assets/database.png" />
      <h1>Database</h1>
    </div>
    <div class="skill-list">
      <div class="detail-skill">MySQL</div>
      <div class="detail-skill">Oracle</div>
      <div class="detail-skill">Firebase</div>
    </div>
  </div>
</template>

<script setup>
import "@/styles/detail-skill.scss"; // CSS 파일을 import
</script>

<style scoped>
.detail-skill:nth-child(1) {
  background-color: #00758f; /* MySQL의 블루 */
}

.detail-skill:nth-child(2) {
  background-color: #ff5722; /* Oracle의 오렌지 */
}

.detail-skill:nth-child(3) {
  background-color: #0d47a1; /* Firebase의 파란색 */
}
</style>
