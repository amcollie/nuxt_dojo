<template>
  <header class="shadow-sm bg-white">
    <nav class="container mx-auto p-4">
      <NuxtLink 
        to="/products"
        class="font-bold"
      >
        Nuxt Dojo Merch
      </NuxtLink>
      
    </nav>
  </header>

  <main class="container mx-auto p-4">
    <slot />
  </main>

<footer class="container mx-auto p-4 flex justify-between border-t-2">
  <nav>
    <ul class="flex gap-4">
        <li>
          <NuxtLink to="/">
            Home
          </NuxtLink>
        </li>
        <li>
          <NuxtLink to="/about">
            About Us
          </NuxtLink>
        </li>
        <li>
          <NuxtLink to="/products">
            Products
          </NuxtLink>
        </li>
      </ul>
  </nav>
</footer>
</template>

<style scoped>
  .router-link-exact-active {
    color: #12b488;
  }
</style>