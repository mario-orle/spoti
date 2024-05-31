<script setup lang="ts">
</script>

<template>
  <div class="view">
    <div class="menu"></div>
    <div class="library"></div>
    <div class="main">
      <RouterView />
    </div>
    <div class="player"></div>
  </div>
</template>

<style scoped lang="scss">
.view {
  height: 100%;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(3, 1fr);
  grid-column-gap: 5px;
  grid-row-gap: 6px;
  .menu {
    grid-area: 1 / 1 / 2 / 2;
    background-color: #fabada;
  }
  .library {
    grid-area: 2 / 1 / 3 / 2;
    background-color: #cebada;
  }
  .main {
    grid-area: 1 / 2 / 3 / 3;
    background-color: #facada;
  }
  .player {
    grid-area: 3 / 1 / 4 / 3;
    background-color: #fabaca;
  }
}
</style>
