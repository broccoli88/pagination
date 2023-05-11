<script setup></script>
<template>
  <div>
    <h2>Pagination Component</h2>
    <button class="pagination-btn">Previous</button>
    <span class="pagination-row" v-for="(item, index) in new Array(10)" :key="index">
      <button class="pagination-btn">{{ index + 1 }}</button>
    </span>
    <button class="pagination-btn">Next</button>
    <slot />
  </div>
</template>

<style scoped>
h2 {
  margin-bottom: 2rem;
}
.pagination-btn {
  font-size: 1.5rem;
  margin-right: 0.5rem;
  padding: 0.5rem;
  border-radius: 4px;
  border: none;
  cursor: pointer;
}
</style>
