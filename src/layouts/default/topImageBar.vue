<template>
  <div class="background-container"></div>
</template>

<script setup>
//
</script>

<style scoped>
/* 기본 스타일 */
.background-container {
  background-image: url("/topImage.png"); /* public 폴더에서 이미지 사용 */
  background-size: cover; /* 이미지가 화면 크기에 맞게 조정 */
  background-position: center center; /* 이미지 중앙에 위치 */
  background-repeat: no-repeat; /* 이미지 반복 방지 */

  width: 100%; /* 화면 너비에 맞게 설정 */
  height: 50vh; /* 화면 높이에 비례해서 설정 (40% 높이) */
  position: relative; /* 위치 설정을 위한 속성 */
}

/* 화면 너비가 1024px 이하일 때 적용 */
@media (max-width: 1024px) {
  .background-container {
    background-position: center -100px; /* 배경 위치 조정 */
    height: 40vh; /* 화면 높이에 비례하여 높이를 50%로 설정 */
  }
}

/* 화면 너비가 768px 이하일 때 적용 */
@media (max-width: 768px) {
  .background-container {
    background-position: center -50px; /* 배경 위치 조금 더 조정 */
    height: 25vh; /* 화면 높이에 비례하여 높이를 60%로 설정 */
  }
}

/* 화면 너비가 480px 이하일 때 적용 */
@media (max-width: 480px) {
  .background-container {
    background-position: center center; /* 배경 이미지를 화면의 중앙에 고정 */
    height: 20vh; /* 화면 높이에 비례하여 높이를 70%로 설정 */
  }
}
</style>
