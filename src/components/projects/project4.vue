<template>
  <div class="project-card">
    <div class="card-top">
      <div class="card-top-img">
        <img src="/src/assets/gsgs.png" />
      </div>
      <div class="card-top-txt">
        <h4 class="project-title">겸사겸사</h4>
        <div class="project-period">2024.09 (4人 팀 프로젝트)</div>
      </div>
    </div>

    <hr />
    <div class="project-summary">
      <h5 class="project-subtitle">
        “가는 길에, 가는 김에, 당신 곁에”이라는 슬로건으로 사용자들에게<br />새로운
        배송 플랫폼을 제공하는 안드로이드 어플리케이션 프로젝트.
      </h5>
      <ul class="project-details">
        <li>팀장으로서 개발 과정 리드 및 테스트 진행</li>
        <li>안드로이드 스튜디오 기반의 UI/UX 작업 담당</li>
        <li>Tmap API를 활용한 지도 관련 기능 담당</li>
        <li>Firebase의 Realtime DB 활용한 실시간 정보 제공 기능 개발</li>
        <li>배송건에 대한 CRUD 작업</li>
      </ul>
    </div>
    <div class="project-url">
      관련 링크 :
      <a href="" target="_blank">배포 웹 사이트</a>
      <a href="" target="_blank">Github 링크</a>
      <a href="" target="_blank">프로젝트 시연 영상</a>
    </div>
    <hr />
    <div class="project-tech-stacks">
      <div class="detail-skill">Kotlin</div>
      <div class="detail-skill">Firebase</div>
      <div class="detail-skill">Android Studio</div>
      <div class="detail-skill">Github</div>
      <div class="detail-skill">···</div>
    </div>
  </div>
</template>

<script setup>
import "@/styles/project-css.scss"; // CSS 파일을 import
</script>

<style scoped>
.detail-skill:nth-child(1) {
  background-color: #9994ff;
}
.detail-skill:nth-child(2) {
  background-color: #6bc7eb;
}
.detail-skill:nth-child(3) {
  background-color: #4caf50;
}
.detail-skill:nth-child(4) {
  background-color: #00758f;
}
.detail-skill:nth-child(5) {
  background-color: #9e9e9e;
}
</style>
