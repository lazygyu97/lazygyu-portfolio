<template>
  <div class="skill">
    <div class="language">
      <img src="/src/assets/api.png" />
      <h1>Backend</h1>
    </div>
    <div class="detail-skill">a</div>
    <div class="detail-skill">b</div>
    <div class="detail-skill">c</div>
    <div class="detail-skill">d</div>
  </div>
</template>

<script setup></script>

<style scoped>
.skill {
  display: flex; /* 한 줄로 정렬 */
  align-items: flex-start; /* 수직 가운데 정렬 */

  gap: 20px; /* 요소 간 간격 */

  width: 80%;
}

.language {
  display: flex;
  align-items: center;
  column-gap: 1rem;
  flex-shrink: 0;
  width: 10rem;
  font-weight: 900;
  height: 100%;
}

.language > img {
  width: 30px;
}

.language > h1 {
  margin: 0; /* 기본 마진 제거 */
  font-size: 20px;
}

.detail-skill {
  display: inline-flex; /* 텍스트 길이에 따라 크기 조정 가능 */
  justify-content: center; /* 수평 가운데 정렬 */
  align-items: center; /* 수직 가운데 정렬 */
  width: auto; /* 텍스트 길이에 따라 너비 조정 */
  height: 35px;
  border-radius: 10px; /* 둥근 모서리 */
  color: white; /* 텍스트 색상 */
  font-weight: bold; /* 텍스트 강조 */
  padding: 0 20px; /* 좌우 여백 추가 */
  text-align: center;
  white-space: nowrap; /* 텍스트 줄바꿈 방지 */
}

.detail-skill:nth-child(2) {
  background-color: #ff6b6b; /* 빨강 */
}

.detail-skill:nth-child(3) {
  background-color: #6bcff6; /* 파랑 */
}

.detail-skill:nth-child(4) {
  background-color: #ffd93d; /* 노랑 */
}

.detail-skill:nth-child(5) {
  background-color: #81c784; /* 초록 */
}
</style>
