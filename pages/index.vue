<template>
  <section class="h-screen relative">
    <div aria-hidden="true" class="absolute inset-0 grid grid-cols-2 -space-x-52 opacity-40 dark:opacity-20">
        <div class="blur-[106px] h-56 bg-gradient-to-br from-primary to-purple-400 dark:from-blue-700"></div>
        <div class="blur-[106px] h-32 bg-gradient-to-r from-cyan-400 to-sky-300 dark:to-indigo-600"></div>
    </div>
    <div class="text-center flex flex-col justify-center items-center h-screen">
      <h1 class="font-extrabold text-6xl md:text-9xl [text-wrap:balance] bg-clip-text text-transparent bg-gradient-to-r from-slate-200/60 to-50% to-slate-200 mb-20">Summand</h1>
      <h3 class="font-semibold text-3xl md:text-3xl bg-clip-text text-transparent bg-gradient-to-r from-slate-200/60 to-50% to-slate-200">New Generation CLI</h3>
    </div>

  </section>
  <section class="h-screen">
    
  </section>
</template>

<script setup>
import { useDark, useToggle } from "@vueuse/core";

const isDark = useDark();
const toggleDark = useToggle(isDark);
</script>

<style scoped>

</style>