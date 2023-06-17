<template>
  <div>
    <header class="shadow-sm bg-white">
      <nav class="container mx-auto p-4">
        <NuxtLink to="/products" class="font-bold">Gary's Merch</NuxtLink>
      </nav>
    </header>

    <!-- output our page content -->
    <div class="container mx-auto p-4">
      <slot></slot>
    </div>

    <footer class="container mx-auto p-4 flex justify-between border-t-2">
      <ul class="flex gap-4">
        <li><NuxtLink to="/">主頁</NuxtLink></li>
        <li><NuxtLink to="/about">關於</NuxtLink></li>
        <li><NuxtLink to="/products">商品</NuxtLink></li>
      </ul>
    </footer>
  </div>
</template>

<style scoped>
.router-link-exact-active {
  color: #4bbebe;
}
</style>
