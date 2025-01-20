<template>
  <v-app>
    <default-bar />
    <v-main class="main-container">
      <!-- 각 영역을 개별 섹션으로 구성 -->
      <section class="snap-section">
        <middle-area1 />
      </section>
      <section class="snap-section">
        <middle-area2 />
      </section>
      <section class="snap-section">
        <middle-area3 />
      </section>
      <section class="snap-section">
        <middle-area4 />
      </section>
      <section class="snap-section-big">
        <middle-area5 />
        <bottom-bar />
      </section>

      <!-- 최상단으로 이동 버튼 -->
      <button class="scroll-to-top" v-show="showScrollTop" @click="scrollToTop">
        ↑
      </button>
    </v-main>
  </v-app>
</template>

<script setup>
import { ref, onMounted, onBeforeUnmount } from "vue";

import DefaultBar from "./AppBar.vue";
import MiddleArea1 from "./topImageBar.vue";
import MiddleArea2 from "./aboutMe.vue";
import MiddleArea3 from "./skill.vue";
import MiddleArea4 from "./archiving.vue";
import MiddleArea5 from "./project.vue";
import BottomBar from "./bottom-bar.vue";

// 스크롤 상태
const showScrollTop = ref(false);

// 최상단으로 스크롤 이동 함수
const scrollToTop = () => {
  const mainContainer = document.querySelector(".main-container"); // main-container 선택
  if (mainContainer) {
    mainContainer.scrollTo({
      top: 0,
      behavior: "smooth", // 부드럽게 스크롤
    });
  } else {
    window.scrollTo({
      top: 0,
      behavior: "smooth", // 부드럽게 스크롤
    });
  }
};

// 스크롤 이벤트 핸들러
const handleScroll = (e) => {
  showScrollTop.value = e.target.scrollTop > 200; // main-container 스크롤 확인
};

onMounted(() => {
  const mainContainer = document.querySelector(".main-container");
  mainContainer.addEventListener("scroll", handleScroll);
});

onBeforeUnmount(() => {
  const mainContainer = document.querySelector(".main-container");
  mainContainer.removeEventListener("scroll", handleScroll);
});
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box; /* 박스 크기를 요소의 전체 크기로 계산 */
}

html,
body {
  height: 100%; /* 페이지가 화면을 꽉 채우도록 설정 */
}
/* 전체 컨테이너에 스크롤 스냅 활성화 */
.main-container {
  height: 100vh; /* 전체 화면 높이 */
  scroll-snap-type: y mandatory; /* 세로 스크롤 스냅 설정 */
  overflow-y: scroll; /* 세로 스크롤 활성화 */
  scroll-behavior: smooth; /* 부드러운 스크롤 효과 */
  display: flex;
  flex-direction: column;
}

/* 각 영역의 스냅 섹션 */
.snap-section {
  height: 50vh; /* 각 섹션 높이 */
  scroll-snap-align: start; /* 스냅 시작점 */
  display: flex;
  justify-content: center;
  align-items: center;
}

.snap-section-big {
  height: 100vh; /* 프로젝트 섹션은 전체 화면 차지 */
  scroll-snap-align: start; /* 스냅 시작점 */
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

/* 최상단으로 이동 버튼 스타일 */
.scroll-to-top {
  position: fixed;
  bottom: 20px;
  right: 20px;
  z-index: 1000;
  background-color: #676767;
  color: white;
  border: none;
  border-radius: 50%;
  width: 50px;
  height: 50px;
  font-size: 18px;
  font-weight: bold;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  cursor: pointer;
  transition: opacity 0.3s, transform 0.3s;
  opacity: 0.8;
}

.scroll-to-top:hover {
  opacity: 1;
  transform: scale(1.1);
}

/* 반응형 디자인 */
@media (max-width: 768px) {
  /* 모바일 화면에서 각 섹션 높이 조정 */
  .snap-section,
  .snap-section-big {
    width: 100%;
    height: auto; /* 높이를 자동으로 설정 */
  }

  /* 프로젝트 섹션 조정 */
  .snap-section-big {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  /* 최상단 버튼 크기 조정 */
  .scroll-to-top {
    width: 40px;
    height: 40px;
    font-size: 16px;
  }
}

@media (max-width: 480px) {
  /* 모바일 화면에서 각 섹션의 높이와 배치가 자동으로 맞춰짐 */
  .snap-section,
  .snap-section-big {
    height: auto;
  }

  /* 최상단 버튼 크기 조정 */
  .scroll-to-top {
    width: 35px;
    height: 35px;
    font-size: 14px;
  }
}
</style>
