<script setup lang="ts">
import { ref } from 'vue'
import HorizontalScroll from './components/HorizontalScroll.vue'
const showExtraContent = ref(false)
</script>

<template>
  <HorizontalScroll class="content">
    <h1>Scroooooooooooooooooooooooooooooooooooolling</h1>
    <p v-if="showExtraContent">
      Even more
      scrooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooooolling
    </p>
    <p>More content</p>
    <p>More content</p>
    <p>More content</p>
    <p>More content</p>
    <p>More content</p>
    <p>More content</p>
    <p>More content</p>
  </HorizontalScroll>
  <button class="btn" @click="showExtraContent = !showExtraContent">Toggle extra content</button>
</template>

<style scoped>
.content {
  border: 2px solid;
  width: 100%;
}
.btn {
  margin-top: 10px;
  border: 5px solid #e0e0e0;
  border-radius: 10px;
  padding: 10px;
}
</style>
