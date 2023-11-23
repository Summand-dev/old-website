<template>
  <div class="bg-slate-900 border-2 border-indigo-950 flex flex-col justify-center items-center p-10 rounded-2xl">
    <div class="text-center text-white text-sm font-normal mb-2">{{ author }}</div>
    <div class="text-center text-neutral-200 text-xs font-normal"><slot/></div>
  </div>
</template>

<script setup lang="ts">
  const props = defineProps({
    author: String
  });
</script>