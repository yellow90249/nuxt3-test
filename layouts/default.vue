<template>
  <div>
    <header class="shadow-sm bg-white">
      <nav class="container mx-auto p-4 flex justify-between">
        <NuxtLink to="/" class="font-bold text-xl logo">GaryDev</NuxtLink>
        <ul class="flex gap-4">
          <li><NuxtLink to="/">主頁</NuxtLink></li>
          <li><NuxtLink to="/about">關於</NuxtLink></li>
          <li><NuxtLink to="/products">商品</NuxtLink></li>
        </ul>
      </nav>
    </header>

    <!-- output our page content -->
    <div class="container mx-auto p-4">
      <slot></slot>
    </div>
  </div>
</template>

<style scoped>
.router-link-exact-active,
.logo {
  color: #4bbebe;
}
</style>
