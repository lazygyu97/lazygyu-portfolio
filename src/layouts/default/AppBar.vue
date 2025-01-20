<template>
  <v-app-bar flat>
    <div class="custom-container">
      <h1>Lazygyu's Portfolio</h1>

      <!-- 여백을 추가해 오른쪽으로 밀기 -->
      <v-spacer></v-spacer>
    </div>
  </v-app-bar>
</template>

<script setup>
//
</script>

<style scoped>
h1 {
  font-style: normal;
  font-size: 25px;
}
.custom-container {
  margin: 0 auto;
  padding: 0 20px;
  min-width: 1550px;
  display: flex;

  justify-content: flex-start;
  align-items: center;
  text-align: center;
}

/* 앱바 하단에 얇은 그림자 추가 */
.v-app-bar {
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); /* 그림자 효과 */
}
</style>
