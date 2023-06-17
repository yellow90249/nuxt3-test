<template>
  <div>
    <header>
      <NuxtLink to="/">Nuxt Dojo</NuxtLink>
      <ul>
        <li><NuxtLink to="/">Home</NuxtLink></li>
        <li><NuxtLink to="/about">About</NuxtLink></li>
        <li><NuxtLink to="/product">Product</NuxtLink></li>
      </ul>
    </header>

    <!-- output our page content -->
    <div>
      <slot></slot>
    </div>
  </div>
</template>

<style scoped>
.router-link-exact-active {
  color: #12b488;
}
</style>
