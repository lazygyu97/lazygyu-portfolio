<template>
  <div class="board-layer">
    <div class="image-container">
      <img src="/src/assets/notion.png" alt="Background Image" />
    </div>
    <div class="link-container">
      <a
        href="#"
        @click="showAlert('작업중입니다', $event)"
        class="link"
        style="margin-right: 10px"
        >이력서 관련 문서</a
      >
      <a>/</a>
      <a
        href="#"
        @click="showAlert('작업중입니다', $event)"
        class="link"
        style="margin-left: 10px"
        >기술 문서</a
      >
    </div>
    <div class="description-container">
      <p class="description">각종 문서 저장소</p>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    showAlert(message, event) {
      alert(message); // 알림 표시
    },
  },
};
</script>

<style scoped>
.board-layer {
  /* 부모 컨테이너 스타일 */
  width: 100%; /* 너비를 100%로 설정하여 유동적으로 변경 */
  max-width: 400px; /* 최대 너비 설정 */
  height: 400px;
  background: #ffffff;
  border-radius: 20px;
  display: flex;
  flex-direction: column; /* 수직 배치 */
  align-items: flex-start; /* 자식 요소 좌측 정렬 */
  padding: 20px; /* 내부 여백 */
  box-sizing: border-box; /* 여백이 전체 크기에 포함되도록 설정 */
  margin-bottom: 20px; /* 카드 간 간격 */
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

/* 반응형 설정: 화면이 600px 이하일 때 */
@media (max-width: 600px) {
  .board-layer {
    width: 100%; /* 화면이 좁을 때 카드의 너비를 100%로 설정 */
    margin-bottom: 20px; /* 카드 간 간격 */
  }

  .image-container img {
    height: 120px; /* 작은 화면에서는 이미지의 높이를 줄임 */
  }

  .description {
    font-size: 12px; /* 작은 화면에서는 글자 크기를 줄임 */
  }
}
</style>
