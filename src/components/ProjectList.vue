<template>
    <div>
        <h2>Ingresa tu Proyecto</h2>
        <label for="">Título del Proyecto</label>
        <input type="text">
        <label for="">Prioridad</label>
        <input type="text">
        <label for="">Prioridad</label>
        <input type="text">
        <slot name="header"></slot>
        <ul>
        <ProjectItem v-bind="projct" v-for="(projct, index) in projects" :key="index"/>
        </ul>
    </div>
</template>

<script setup lang="ts">
import { ProjectData } from '@/data/ProjectData';
import ProjectItem from './ProjectItem.vue';
import {ref} from 'vue';

const projectName = ref('')

const projects = ref(ProjectData)
</script>

<style>

</style>