<template>
<div>
    <h1 class="text-3xl font-bold underline text-center text-green-300">Summand</h1>

    <h1 class="text-3xl font-bold text-center mt-12 mb-12">What people say</h1>
    <Swiper :modules="[SwiperAutoplay, SwiperNavigation]" :slides-per-view="3" :loop="true" :autoplay="{ delay: 8000, disableOnInteraction: true }" :navigation="true"  :centeredSlides="true">
        <SwiperSlide v-for="i in 10" class="p-12">
            <div class="swiper-slide-content">
            <RecommandationCard class="recommandation-card"></RecommandationCard>
            </div>
        </SwiperSlide>
    </Swiper>

</div>
</template>

<script setup>

</script>

<style>

.swiper-slide {
  @apply blur-[2px]
}

.swiper-slide-active {
  @apply blur-0;
  @apply  scale-110;
}

</style>