<script setup lang="ts">
import CollectionItem from '@/components/_collection/CollectionItem.vue'
import { computed } from 'vue'
const gridRowCount = computed(() => {
  return Math.ceil(9 / 3)
})
</script>

<template>
  <div class="collection">
    <CollectionItem v-for="item in 16" title="模块查看系统" :key="item" :arguments="{ name: true }">
      <div style="font-size: 46px">难难啊难,这里面放置组件</div>
    </CollectionItem>
  </div>
</template>

<style lang="scss">
.collection {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  min-height: 40vh;
  grid-template-rows: repeat(v-bind(gridRowCount), 1fr);
}

.collection-item {
  height: 28vh;
}
</style>

<script lang="ts">
export default { name: 'CollectionIndex' }
</script>
