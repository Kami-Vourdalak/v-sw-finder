<template>
  <div class="h-screen w-full bg-neutral-900 text-gray-50">
    <div class="flex justify-center items-center h-24 pl-4">
      <h1 class="text-3xl font-bold">Star Wars Finder</h1>
    </div>
    <div class="pl-4 pt-4">
      <slot />
    </div>
  </div>
</template>
<script lang="ts">
export default {
  name: "TheLayout",
};
</script>
