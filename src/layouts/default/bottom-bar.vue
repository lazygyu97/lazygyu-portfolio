<template>
  <div class="bottom">
    <div class="bottom-txt">
      <h3>@ 2025. Park Hyeon Gyu. All rights reserved.</h3>
      <h3>이 사이트는 홈 서버를 구축하여 배포하고 있습니다.</h3>
    </div>
  </div>
</template>

<script setup>
//
</script>

<style scoped>
.bottom {
  width: 100%;
  height: 3vh;
  background-color: rgb(33, 33, 33);
  text-align: center;
  color: white;
  display: flex; /* flexbox 활성화 */
  justify-content: center; /* 가로 중앙 정렬 */
  align-items: center; /* 세로 중앙 정렬 */
}

.bottom-txt {
  font-size: 12px; /* 원하는 글자 크기 입력 */
}
@media (max-width: 768px) {
  .bottom-txt {
    font-size: 9px; /* 원하는 글자 크기 입력 */
  }
}
@media (max-width: 600px) {
  .bottom-txt {
    font-size: 5px; /* 원하는 글자 크기 입력 */
  }
}
</style>
