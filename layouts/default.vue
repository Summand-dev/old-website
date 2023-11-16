<template>

    <div class="flex justify-center items-center">
      <Navbar/>
    </div>
    <div class="h-screen">
      <slot />
    </div>

    <div class="container mx-auto">
      <Footer />
    </div>
    
</template>

<script setup>
import Navbar from '@/components/navbar.vue'
import Footer from '@/components/footer.vue'
</script>

<style scoped>
</style>