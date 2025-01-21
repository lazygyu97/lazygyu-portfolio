<template>
  <div class="project-card">
    <div class="card-top">
      <div class="card-top-img">
        <img src="/src/assets/seoulmate.png" />
      </div>
      <div class="card-top-txt">
        <h4 class="project-title">Seoul Mate</h4>
        <div class="project-period">2024.09 (4人 팀 프로젝트)</div>
      </div>
    </div>

    <hr />
    <div class="project-summary">
      <h5 class="project-subtitle">
        서울시에서 제공하는 공공 서비스 데이터를 사용자들에게 편리하게 제공하는
        서비스 개발 프로젝트.
      </h5>
      <ul class="project-details">
        <li>팀장으로서 개발 계획, 일정 산정, 개발 및 테스트, 배포 진행</li>
        <li>서울시 공공 API 활용 로직 작업</li>
        <li>사용자의 관심 목록 CRUD 작업</li>
        <li>이메일, 전화번호 인증 로직 작업</li>
        <li>AWS 리눅스 배포 및 CI/CD 파이프라인</li>
        <li>Vue.js 를 기반으로 프론트엔드 작업</li>
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
      <div class="detail-skill">Java</div>
      <div class="detail-skill">Spring Boot</div>
      <div class="detail-skill">Spring Security</div>
      <div class="detail-skill">Redis</div>
      <div class="detail-skill">MySQL</div>
      <div class="detail-skill">JPA</div>
      <div class="detail-skill">AWS</div>
      <div class="detail-skill">Vue.js</div>
      <div class="detail-skill">···</div>
    </div>
  </div>
</template>

<script setup>
import "@/styles/project-css.scss"; // CSS 파일을 import
</script>

<style scoped>
.detail-skill:nth-child(1) {
  background-color: #f44336;
}

.detail-skill:nth-child(2) {
  background-color: #4caf50;
}

.detail-skill:nth-child(3) {
  background-color: #6bc7eb;
}
.detail-skill:nth-child(4) {
  background-color: #ff7043;
}
.detail-skill:nth-child(5) {
  background-color: #00758f;
}
.detail-skill:nth-child(6) {
  background-color: #4caf50;
}
.detail-skill:nth-child(7) {
  background-color: #00acc1;
}
.detail-skill:nth-child(8) {
  background-color: #9994ff;
}
.detail-skill:nth-child(9) {
  background-color: #9e9e9e;
}
</style>
