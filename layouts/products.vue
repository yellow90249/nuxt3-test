<template>
  <div>
    <header>
      <NuxtLink to="/products">Nuxt Dojo Merch</NuxtLink>
    </header>

    <!-- output our page content -->
    <div>
      <slot></slot>
    </div>

    <footer>
      <ul>
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="/about">About</NuxtLink></li>
        <li><NuxtLink to="/product">Product</NuxtLink></li>
      </ul>
    </footer>
  </div>
</template>

<style scoped>
.router-link-exact-active {
  color: #12b488;
}
</style>
