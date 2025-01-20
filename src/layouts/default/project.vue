<template>
  <div class="custom-container">
    <div style="margin-bottom: 20px; margin-top: 80px"><h1>PROJECTS</h1></div>

    <v-row class="projects" justify="center" wrap>
      <!-- 각 카드 컴포넌트를 v-col로 감싸기 -->
      <v-col v-for="n in 6" :key="n" cols="12" sm="6" md="4">
        <!-- 각 프로젝트 컴포넌트 -->
        <component :is="'Project' + n" />
      </v-col>
    </v-row>
  </div>
</template>

<script setup>
// 각 프로젝트 컴포넌트를 임포트합니다.
import Project1 from "@/components/projects/project1.vue";
import Project2 from "@/components/projects/project2.vue";
import Project3 from "@/components/projects/project3.vue";
import Project4 from "@/components/projects/project4.vue";
import Project5 from "@/components/projects/project5.vue";
import Project6 from "@/components/projects/project6.vue";

// 컴포넌트 등록
defineOptions({
  components: {
    Project1,
    Project2,
    Project3,
    Project4,
    Project5,
    Project6,
  },
});
</script>

<style scoped>
.custom-container {
  margin: 0 auto;
  padding: 0 20px;
  max-width: 1550px;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  text-align: center;
  min-height: 97vh; /* 화면을 벗어나지 않도록 설정 */
}

.projects {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

/* 각 카드 컴포넌트의 스타일 */
.v-col {
  margin-bottom: 30px;
}

/* 미디어 쿼리: 작은 화면에서 한 줄에 하나씩 보이도록 설정 */
@media (max-width: 600px) {
  .v-col {
    max-width: 100%; /* 한 줄에 하나씩 표시되도록 설정 */
    padding: 0 10px; /* 카드 간 간격 조정 */
  }
}
</style>
