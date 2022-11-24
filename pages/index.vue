<template>
  <main>
    <h1>Home page</h1>
    <NuxtLink to="/about">
      About (internal link that belongs to the Nuxt App)
    </NuxtLink>
    <a href="https://nuxtjs.org">External Link to another page</a>
    <NuxtLink to="/about" no-prefetch>About page not pre-fetched</NuxtLink>
    <NuxtLink to="/about" :prefetch="false">About page not pre-fetched</NuxtLink>

  </main>
</template>
<style>
.nuxt-link-active {
  color: red;
}

.nuxt-link-exact-active {
  color: green;
}
</style>