<template>
<div>
    <h1 class="text-3xl font-bold underline text-center text-green-300">Summand</h1>

    <h1 class="text-3xl font-bold text-center mt-12 mb-12">What people say</h1>
    <Swiper :options="swiperOptions" :loop="true" :autoplay="{ delay: 8000, disableOnInteraction: true }" :navigation="true"  :centeredSlides="true" :slides-per-view="3">
        <SwiperSlide v-for="i in 10">
          <RecommandationCard author="Ahmad">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut nemo veniam nostrum? Officiis voluptates optio provident tempora, delectus iste laborum modi enim! Impedit est sapiente ea quo optio, praesentium quae.</RecommandationCard>
        </SwiperSlide>
    </Swiper>

</div>
</template>

<script setup>
const swiperOptions = {
  modules:[SwiperAutoplay, SwiperNavigation],
  breakpoints: {
    640: {
      slidesPerView: 1,
    },
  },
};
</script>

<style>

.swiper-slide {
  @apply blur-[2px] transition px-16; 
}

.swiper-slide-active {
  @apply blur-0 scale-110 transition;
}

.swiper-button-next, .swiper-button-prev {
  @apply border-2 text-indigo-500 border-indigo-500 rounded-full w-10 h-10 flex items-center justify-center;
}

.swiper-button-next::after, .swiper-button-prev::after {
  @apply text-xl; 
}

</style>

