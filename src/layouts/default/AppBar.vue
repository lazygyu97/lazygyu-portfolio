<template>
  <v-app-bar flat>
    <div class="custom-container">
      <v-app-bar-title>
        Lazygyu's Portfolio
      </v-app-bar-title>

      <!-- 여백을 추가해 오른쪽으로 밀기 -->
      <v-spacer></v-spacer>

      <!-- 아이콘을 오른쪽 끝에 배치 -->
      <v-icon icon="mdi-circle-slice-4" />
    </div>
  </v-app-bar>
</template>

<script setup>
//
</script>

<style scoped>
.custom-container {
  margin: 0 auto;
  min-width: 1550px;
  display: flex; /* 내부 요소를 flexbox로 정렬 */
  align-items: center; /* 수직 가운데 정렬 */
}
</style>
