<script setup>
import { ref } from 'vue'

defineProps({
  msg: String,
})

const count = ref(0)
</script>

<template>
  <div class="dashboard">
    <div class="top-container mb-4 row g-0 rounded-4">
      <div class="col-8 border-end border-3">
        <div class="row justify-content-between">
          <div class="col p-4">Expense $</div>
          <div class="col p-4">Income $</div>
          <div class="col p-4">Net $</div>
        </div>
        <div class="row">
          <div class="col p-4">Line/Bar/Donut Graph</div>
        </div>
      </div>
      <div class="col p-4">
        Latest Transactions
      </div>
    </div>
    <div class="categories-container row">
      <div class="col">
        <div class="category-card p-4 rounded-4">Category 1</div>
      </div>
      <div class="col">
        <div class="category-card p-4 rounded-4">Category 2</div>
      </div>
      <div class="col">
        <div class="category-card p-4 rounded-4">Category 3</div>
      </div>
      <div class="col">
        <div class="category-card p-4 rounded-4">Category 4</div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="scss">
  .top-container {
    background-color: #FEFEFF;
    height: 500px;
  }

  .category-card {
    background-color: #FEFEFF;
    height: 150px;
  }

</style>
