<template>
  <ProductDetail :product="product"></ProductDetail>
</template>

<script setup>
const { id } = useRoute().params;
const url = 'https://fakestoreapi.com/products/' + id;

// fetch the product
const { data: product } = await useFetch(url);

if (!product.value) {
  throw createError({ statusCode: 404, statusMessage: 'Product not found' });
}
</script>

<style lang="scss" scoped></style>
