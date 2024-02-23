<template>
  <div class="card">
    <span>
        <h3>{{ props.id }}</h3>
        <h3>{{ props.title }}</h3>
        <h3>{{ props.priority }}</h3>
        <h3>{{ props.completed }}</h3>
    </span>
  </div>
</template>

<script setup lang="ts">
import type { IProject } from '@/interfaces/IProject';

const props = defineProps<IProject>()
</script>

<style></style>
