<script setup>
const items = new Array(1000000).fill({ id: 0, name: "Item" });
</script>

<template>
  <div>
    <NuxtWelcome />
    <div>
      <div v-for="item in items" :key="item.id">
        <!-- Content here -->
      </div>
    </div>
  </div>
</template>
