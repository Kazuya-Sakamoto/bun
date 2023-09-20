<script setup>
const items = new Array(100000).fill({ id: 0, name: "Item" });
</script>

<template>
  <div>
    <NuxtWelcome />
    <div>
      <div v-for="item in items" :key="item.id">s</div>
    </div>
  </div>
</template>
