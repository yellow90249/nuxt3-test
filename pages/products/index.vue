<template>
  <div>
    <div class="grid gap-5 grid-cols-1 md:grid-cols-2 lg:grid-cols-4">
      <div v-for="p in products">
        <ProductCard :product="p"></ProductCard>
      </div>
    </div>
  </div>
</template>

<script setup>
// fetch the products
const { data: products } = await useFetch('https://fakestoreapi.com/products');
useHead({
  title: 'GaryDev | 商品',
});
</script>

<style lang="scss" scoped></style>
