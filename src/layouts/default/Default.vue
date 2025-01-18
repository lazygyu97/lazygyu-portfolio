<template>
  <v-app>
    <default-bar />
    <v-main>
      <middle-area1 />
      <middle-area2 />
      <middle-area3 />
      <middle-area4 />
      <middle-area5 />
      <bottom-bar />
    </v-main>
  </v-app>
</template>

<script setup>
import DefaultBar from "./AppBar.vue";
import MiddleArea1 from "./topImageBar.vue";
import MiddleArea2 from "./aboutMe.vue";
import MiddleArea3 from "./skill.vue";
import MiddleArea4 from "./archiving.vue";
import MiddleArea5 from "./project.vue";
import BottomBar from "./bottom-bar.vue";
</script>
