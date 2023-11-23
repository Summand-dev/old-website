<template>
<div>
    <h1 class="text-3xl font-bold underline text-center text-green-300">Summand</h1>

    <h1 class="text-3xl font-bold text-center mt-12 mb-12">What people say</h1>

    <div class="flex">
      <svg
        class="custom-button-prev relative w-2/12 md:w-1/12 h-10 md:h-12 mx-auto my-auto cursor-pointer"  viewBox="0 0 49 48" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path id="Vector" d="M24.3409 44C35.3866 44 44.3409 35.0457 44.3409 24C44.3409 12.9543 35.3866 4 24.3409 4C13.2952 4 4.34094 12.9543 4.34094 24C4.34094 35.0457 13.2952 44 24.3409 44Z" stroke="#587DFF" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
        <path id="Vector_2" d="M26.8609 31.0599L19.8209 23.9999L26.8609 16.9399" stroke="#587DFF" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>

      <Swiper 
        class="relative w-8/12 md:w-10/12 mx-auto flex flex-row"
        :modules="[SwiperAutoplay, SwiperNavigation]"
        :navigation="{ nextEl: '.custom-button-next', prevEl: '.custom-button-prev' }"
        :breakpoints="{640:{slidesPerView:3, spaceBetween:15}}"
        :loop="true"  :autoplay="{ delay: 8000, disableOnInteraction: true }" 
        :centeredSlides="true"
        :slides-per-view="1">

          <SwiperSlide v-for="i in 10">
            <RecommandationCard author="Ahmad">Lorem ipsum dolor sit amet consectetur adipisicing elit. Ut nemo veniam nostrum? Officiis voluptates optio provident tempora, delectus iste laborum modi enim! Impedit est sapiente ea quo optio, praesentium quae.</RecommandationCard>
          </SwiperSlide>

      </Swiper>

      <svg
        class="relative w-2/12 md:w-1/12 h-10 md:h-12 mx-auto my-auto custom-button-next cursor-pointer" viewBox="0 0 49 48" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path id="Vector" d="M24.9277 44C35.9734 44 44.9277 35.0457 44.9277 24C44.9277 12.9543 35.9734 4 24.9277 4C13.882 4 4.92773 12.9543 4.92773 24C4.92773 35.0457 13.882 44 24.9277 44Z" stroke="#587DFF" stroke-width="1.5" stroke-miterlimit="10" stroke-linecap="round" stroke-linejoin="round"/>
        <path id="Vector_2" d="M22.4077 31.0599L29.4477 23.9999L22.4077 16.9399" stroke="#587DFF" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
      </svg>

  </div>

</div>
</template>

<script setup>
</script>

<style>
  .swiper-slide {
    @apply blur-[2px] transition; 
  }

  .swiper-slide-active {
    @apply blur-0 scale-110 transition;
  }

</style>

