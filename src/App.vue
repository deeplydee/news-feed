<script setup>
import RefreshButton from './components/RefreshButton.vue'
import SearchForm from './components/SearchForm.vue'
</script>

<template>
  <div class="header">
    <div class="title-wrap">
      <h1 class="title">Список новостей</h1>
      <RefreshButton />
    </div>
    <SearchForm />
  </div>
</template>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: 1060px;
  max-width: 100%;
  max-height: 76px;
  border-bottom: 1px solid #e5e5e5;
  margin-top: 36px;
  margin-right: 36px;
  margin-left: 36px;
  padding-bottom: 36px;
}

.title-wrap {
  display: flex;
}

.title {
  color: #424242;
  text-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25);
  font-family: Roboto;
  font-size: 36px;
  font-style: normal;
  font-weight: 700;
  line-height: normal;
  margin-right: 47px;
}

@media (max-width: 960px) {
  .header {
    flex-direction: column;
    min-height: 150px;
  }

  .title {
    font-size: 24px;
  }

  .title-wrap {
    display: flex;
    align-items: center;
    justify-content: space-between;
    min-width: 320px;
  }
}
</style>
