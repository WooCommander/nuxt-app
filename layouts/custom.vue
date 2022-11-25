<template>
  <div> Some *custom* layout
    <button @click="enableCustomLayout">Update layout1</button>
    <slot />
  </div>
</template>
<script setup>
function enableCustomLayout() { setPageLayout('default') }
definePageMeta({ layout: false, });
</script>