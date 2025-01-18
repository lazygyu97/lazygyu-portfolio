<template>
  <div class="custom-container">
    <div style="margin-bottom: 100px"><h1>PROJECTS</h1></div>
    <v-row class="projects" justify="center">
      <v-col v-for="n in 6" :key="n" cols="12" sm="6" md="4">
        <v-card>
          <v-card-title>Project {{ n }}</v-card-title>
          <v-card-subtitle>Subtitle for Project {{ n }}</v-card-subtitle>
          <v-card-text> Description of Project {{ n }} goes here. </v-card-text>
          <v-card-actions>
            <v-btn color="primary">View Details</v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script setup>
// Vuetify 컴포넌트 자동 임포트가 활성화되어 있다면 별도의 임포트는 필요없습니다.
// 그러나 명시적으로 컴포넌트를 임포트해야 하는 경우 아래와 같이 작성합니다.
// import { VRow, VCol, VCard, VCardTitle, VCardSubtitle, VCardText, VCardActions, VBtn } from 'vuetify/lib';
</script>

<style scoped>
.custom-container {
  margin: 0 auto;
  padding: 0 20px;
  max-width: 1550px;

  /* Flexbox 설정 */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
  height: 100vh;
}
</style>
