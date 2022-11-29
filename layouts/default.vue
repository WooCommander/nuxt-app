<template>
  <div>
    <TheNavigation />
    <div class="container">
      <TheBody />

      <TheFooter />
    </div>
  </div>
</template>
<script setup>
function enableCustomLayout() { setPageLayout('custom') }
definePageMeta({ layout: false, });
</script>
<style>
.container {
  margin-top: 60px;
  padding: 1em;
  max-width: 960px;
  margin-left: auto;
  margin-right: auto;
}
</style>