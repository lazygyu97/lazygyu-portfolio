<template>
  <div class="board-layer">
    <div class="image-container">
      <img src="/src/assets/github.png" alt="Background Image" />
    </div>
    <div class="link-container">
      <a href="#" class="link">자세히 보기</a>
    </div>
    <div class="description-container">
      <p class="description">지금까지 진행한 프로젝트 소스 코드 저장소</p>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.board-layer {
  /* 부모 컨테이너 스타일 */
  width: 30%;
  height: 400px;
  background: #ffffff;
  border-radius: 20px;
  display: flex;
  flex-direction: column; /* 수직 배치 */
  align-items: flex-start; /* 자식 요소 좌측 정렬 */
  padding: 20px; /* 내부 여백 */
}

.image-container img {
  width: 100%; /* 이미지의 너비를 부모에 맞춤 */
  height: 150px; /* 원하는 높이 설정 */
  object-fit: contain; /* 비율을 유지하면서 지정된 높이와 너비에 맞춤 */
  border-radius: 10px; /* 이미지 둥근 모서리 */
}

.link-container {
  margin-top: 20px; /* 이미지와 링크 간격 */
}

.link {
  color: #007bff; /* 링크 색상 */
  text-decoration: none; /* 밑줄 제거 */
  font-weight: bold; /* 강조 */
  font-size: 16px; /* 크기 */
}

.link:hover {
  text-decoration: underline; /* 마우스 호버 시 밑줄 */
}

.description-container {
  margin-top: 10px; /* 링크와 설명 간격 */
}

.description {
  color: #333333; /* 텍스트 색상 */
  font-size: 14px; /* 글꼴 크기 */
  line-height: 1.5; /* 줄 간격 */
}
</style>
