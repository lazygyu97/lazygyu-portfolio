<template>
  <div class="skill">
    <div class="language">
      <img src="/src/assets/code.png" />
      <h1>Language</h1>
    </div>
    <div class="skill-list">
      <div class="detail-skill">Java</div>
      <div class="detail-skill">JavaScript</div>
      <div class="detail-skill">···</div>
    </div>
  </div>
</template>

<script setup>
import "@/styles/detail-skill.scss"; // CSS 파일을 import
</script>

<style scoped>
.detail-skill:nth-child(1) {
  background-color: #f44336;
}

.detail-skill:nth-child(2) {
  background-color: #2196f3;
}

.detail-skill:nth-child(3) {
  background-color: #9e9e9e;
}
</style>
