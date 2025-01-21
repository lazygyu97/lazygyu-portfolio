<template>
  <div class="project-card">
    <div class="card-top">
      <div class="card-top-img">
        <img src="/src/assets/airygram.png" />
      </div>
      <div class="card-top-txt">
        <h4 class="project-title">Airygram</h4>
        <div class="project-period">2024.09 (4人 팀 프로젝트)</div>
      </div>
    </div>

    <hr />
    <div class="project-summary">
      <h5 class="project-subtitle">
        간단한 SNS 서비스 및 관리자 페이지 개발 프로젝트.
      </h5>
      <ul class="project-details">
        <li>팀장으로서 개발 계획, 일정 산정, 개발 및 테스트, 배포 진행</li>
        <li>서비스 관리자 페이지 기능 개발 담당</li>
        <li>사용자의 관심 목록 CRUD 작업</li>
        <li>S3 기반의 이미지 저장 로직 구현</li>

        <li>AWS 기반 배포 및 도메인 작업</li>
        <li>Html, CSS, JS 기반의 프론트엔드 작업</li>
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
      <div class="detail-skill">Lombok</div>
      <div class="detail-skill">Redis</div>
      <div class="detail-skill">MySQL</div>
      <div class="detail-skill">JPA</div>
      <div class="detail-skill">AWS</div>
      <div class="detail-skill">Html,Css,JS</div>
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
  background-color: #6bc7eb;
}
.detail-skill:nth-child(5) {
  background-color: #ff7043;
}
.detail-skill:nth-child(6) {
  background-color: #00758f;
}
.detail-skill:nth-child(7) {
  background-color: #4caf50;
}
.detail-skill:nth-child(8) {
  background-color: #00acc1;
}
.detail-skill:nth-child(9) {
  background-color: #9994ff;
}
.detail-skill:nth-child(10) {
  background-color: #9e9e9e;
}
</style>
