<template>
  <div class="top-container">
    <div class="custom-container">
      <div style="margin-bottom: 50px">
        <h1 style="color: white">ARCHIVING</h1>
      </div>
      <!-- 수평 배치를 위한 컨테이너 추가 -->
      <div class="board-container">
        <github />
        <notion />
        <youtube />
        <instagram />
      </div>
    </div>
  </div>
</template>

<script setup>
import github from "@/components/archiving/github.vue";
import notion from "@/components/archiving/notion.vue";
import youtube from "@/components/archiving/youtube.vue";
import instagram from "@/components/archiving/instagram.vue";
</script>
<style scoped>
.top-container {
  width: 100%;
  background-color: black;
}

.custom-container {
  margin: 0 auto;
  padding: 0 20px;
  max-width: 1550px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  height: 50vh; /* 높이 수정 */
}

.board-container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: flex-start; /* 세로 정렬을 상단으로 변경 */
  width: 100%;
  flex-wrap: wrap; /* 자동 줄 바꿈 */
  gap: 15px; /* 카드 간의 간격 추가 */
  max-width: 1200px;
  margin: 0 auto; /* 중앙 정렬 */
}

.board-layer {
  width: 100%;
  max-width: 250px; /* 카드 최대 너비 설정 */
  height: 300px;
  background: #ffffff;
  border-radius: 20px;
  margin: 0 auto; /* 중앙 정렬 */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  transition: transform 0.3s ease, box-shadow 0.3s ease; /* 부드러운 전환 효과 추가 */
}

/* 호버 효과 추가 */
.board-layer:hover {
  transform: translateY(-10px); /* 위로 살짝 이동 */
  box-shadow: 0 8px 20px rgba(238, 238, 238, 0.473); /* 그림자 추가 */
  background-color: #f0f0f0; /* 배경색 변경 */
}

/* 미디어 쿼리: 화면 크기가 768px 이하일 때 한 줄에 2개씩 배치 */
@media (max-width: 1040px) {
  .board-container {
    flex-direction: row; /* 가로로 배치 */
    justify-content: space-between; /* 카드 간 간격을 일정하게 유지 */
    gap: 20px; /* 카드 간 간격 조정 */
  }

  .board-layer {
    width: 48%; /* 두 개씩 배치하기 위해 50%보다 적당한 너비 설정 */
    margin: 0 auto; /* 중앙 정렬 */
  }

  .custom-container {
    margin: 0 auto;
    padding: 30px 20px;
    max-width: 1550px;
    background-color: black;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    height: auto; /* 높이 수정 */
    padding-bottom: 50px;
  }
}

/* 미디어 쿼리: 화면 크기가 480px 이하일 때 한 줄에 1개씩 배치 */
@media (max-width: 480px) {
  .board-container {
    flex-direction: column; /* 세로로 배치 */
    align-items: center; /* 중앙 정렬 */
    gap: 20px; /* 카드 간 간격 조정 */
  }

  .board-layer {
    width: 90%; /* 한 줄에 하나씩 배치할 때 90% 너비 설정 */
    margin: 0 auto; /* 중앙 정렬 */
  }
}
</style>
