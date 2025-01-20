<template>
  <div class="background-container">
    <div class="custom-container">
      <div class="top-txt">
        <h1>안녕하세요</h1>
        <h1>같이 밥 먹고 싶은 백엔드 개발자,</h1>
        <h1>박현규입니다.</h1>
      </div>

      <div class="top-img">
        <div class="me"></div>
      </div>
    </div>
  </div>
</template>

<script setup>
// script 내용은 필요없음
</script>

<style scoped>
.custom-container {
  margin: 0 auto;
  padding: 0 20px;

  max-width: 1550px;
  display: flex;
  flex-direction: row;
  height: 50vh; /* 높이 수정 */
  align-items: flex-start; /* 기본적으로 top에 맞춰 배치 */
}

.background-container {
  background-image: url("/src/assets/topBackground.jpeg"); /* public 폴더에서 이미지 사용 */
  background-size: cover; /* 이미지가 화면 크기에 맞게 조정 */
  background-position: center center; /* 이미지 중앙에 위치 */
  background-repeat: no-repeat; /* 이미지 반복 방지 */

  width: 100%; /* 화면 너비에 맞게 설정 */
  height: 50vh; /* 화면 높이에 비례해서 설정 (40% 높이) */
  position: relative; /* 자식 요소의 위치를 상대적으로 설정 */
}

.top-txt {
  width: 50%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center; /* 텍스트 세로 중앙 정렬 */
}

.top-txt > h1 {
  font-size: 3rem;
  margin: 0.5rem 0;
  color: rgb(0, 0, 0); /* 텍스트 색상 추가 */
}

.top-img {
  background-image: url("/src/assets/me.png"); /* public 폴더에서 이미지 사용 */
  background-size: cover; /* 이미지가 화면 크기에 맞게 조정 */
  background-position: center 100px; /* 이미지 중앙에 위치 */
  width: 50%;
  height: 100%;
  display: flex;
  /* justify-content: flex-end; 이미지를 오른쪽 하단에 배치 */
  /* align-items: flex-end; */
}
@media (max-width: 1040px) {
  .top-txt > h1 {
    font-size: 2rem; /* 작은 화면에서 폰트 크기 줄이기 */
  }
}

@media (max-width: 768px) {
  .top-txt > h1 {
    font-size: 1.5rem; /* 작은 화면에서 폰트 크기 줄이기 */
  }

  .top-img {
    background-size: 100% auto; /* 이미지가 화면 크기에 맞게 조정 */
    background-position: center 80%; /* 이미지 중앙에 위치 */
    width: 60%;
    height: 100%;
    display: flex;
  }
}

@media (max-width: 480px) {
  .custom-container {
    height: 30vh;
  }
  .background-container {
    height: 30vh;
  }

  .top-txt > h1 {
    font-size: 0.7rem; /* 작은 화면에서 폰트 크기 줄이기 */
  }
  .top-img {
    background-size: auto 50%; /* 이미지가 화면 크기에 맞게 조정 */
    background-position: center 80%; /* 이미지 중앙에 위치 */
    width: 50%;
    height: 100%;
    display: flex;
  }
}
</style>
