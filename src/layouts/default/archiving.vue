<template>
  <div style="background-color: black">
    <div class="custom-container">
      <div style="margin-bottom: 50px">
        <h1 style="color: white">ARCHIVING</h1>
      </div>
      <!-- 수평 배치를 위한 컨테이너 추가 -->
      <div class="board-container">
        <github />
        <notion />
        <youtube />
      </div>
    </div>
  </div>
</template>

<script setup>
import github from "@/components/archiving/github.vue";
import notion from "@/components/archiving/notion.vue";
import youtube from "@/components/archiving/youtube.vue";
</script>

<style scoped>
.custom-container {
  margin: 0 auto;
  padding: 0 20px;
  max-width: 1550px;
  background-color: black;
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

.board-container {
  /* 수평 배치를 위한 설정 */
  display: flex;
  flex-direction: row; /* 수평으로 배치 */
  justify-content: space-around; /* 요소 간 간격 균등 분배 */
  align-items: center; /* 세로 방향 중앙 정렬 */
  width: 100%; /* 컨테이너 전체 너비 */
}

.board-layer {
  /* 각 요소 스타일 */
  width: 30%;
  height: 400px; /* 높이는 고정 */
  background: #ffffff;
  border-radius: 20px;

  /* Flexbox 설정 */
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
