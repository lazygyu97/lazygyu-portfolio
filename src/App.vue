<template>
  <router-view :class="displaySize"/>
</template>
<script lang="ts" setup>
import { useDisplay } from 'vuetify';
import { computed } from 'vue';
const { name } = useDisplay();
const displaySize = computed(() => {
  switch (name.value) {
    case 'xs':
      return 'xs';
    case 'sm':
      return 'sm';
    case 'md':
      return 'md';
    case 'lg':
      return 'lg';
    case 'xl':
      return 'xl';
  }
  return undefined;
});
</script>