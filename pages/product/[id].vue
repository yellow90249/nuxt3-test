<template>
  <div>detail {{ id }}</div>
</template>

<script setup>
const { id } = useRoute().params;

definePageMeta({
  layout: 'products',
});
</script>

<style lang="scss" scoped></style>
