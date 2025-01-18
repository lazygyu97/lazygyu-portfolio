<template>
  <div style="background-color: #fbfbfb">
    <div class="custom-container">
      <div style="margin-bottom: 100px"><h1>ABOUT ME</h1></div>
      <div class="introduce-layer">
        <Name />
        <Birth />
        <Phone />
      </div>
      <div class="introduce-layer">
        <Location />
        <Email />
        <Study />
      </div>
    </div>
  </div>
</template>

<script setup>
// 컴포넌트 임포트
import Name from "@/components/introduce/name.vue";
import Birth from "@/components/introduce/birth.vue";
import Phone from "@/components/introduce/phone.vue";
import Location from "@/components/introduce/location.vue";
import Email from "@/components/introduce/email.vue";
import Study from "@/components/introduce/study.vue";
</script>

<style scoped>
.custom-container {
  margin: 0 auto;
  padding: 0 20px;
  max-width: 1550px;
  background-color: #fbfbfb;
  /* Flexbox 설정 */
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

.introduce-layer > * {
  flex: 1; /* 각 자식 요소들이 동일한 너비를 가지도록 설정 */
  margin: 0 10px; /* 요소들 간 간격 추가 */
}

.introduce-layer > *:first-child {
  margin-left: 0; /* 첫 번째 요소 왼쪽 여백 없애기 */
}

.introduce-layer > *:last-child {
  margin-right: 0; /* 마지막 요소 오른쪽 여백 없애기 */
}
</style>
