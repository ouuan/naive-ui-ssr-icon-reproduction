<template>
  <n-space vertical align="center">
    <n-result
      :key="key"
      title="change key"
      status="info"
    />
    <n-result
      title="change status"
      :status="key & 1 ? 'success' : 'error'"
    />
    <n-button @click="key += 1">update</n-button>
  </n-space>
</template>

<script setup lang="ts">
import { NSpace, NResult, NButton } from 'naive-ui';

const key = ref(0);
</script>
