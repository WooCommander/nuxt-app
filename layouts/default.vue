<template>
  <div>
    <div>
      <ul>
        <li>
          <NuxtLink to="/">
            Home
          </NuxtLink>
        </li>
        <li>
          <NuxtLink to="/about" no-prefetch>About</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/comments" :prefetch="false">comments</NuxtLink>
        </li>
      </ul>




    </div>
    <button @click="enableCustomLayout">Update layout</button>
    <slot />
  </div>
</template>
<script setup>
function enableCustomLayout() { setPageLayout('custom') }
definePageMeta({ layout: false, });
</script>