<script setup lang="ts">
// import ToDoList from '@C/ToDoList.vue'
// import CollectionItem from '@/components/_collection/CollectionItem.vue'
import { PageLayout } from './layout'
</script>

<template>
  <PageLayout title="脑图绘制" no-side>
    <router-view></router-view>
  </PageLayout>
</template>

<style lang="scss">
@import './styles/Basic.scss';
</style>
