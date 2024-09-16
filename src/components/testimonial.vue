<template>
  <section class="bg-white py-16">
    <div class="container mx-auto px-4 text-center">
      <!-- Heading Section -->
      <p class="text-blue-500 font-bold text-[16px]">
        3940+ Happy Landingfolio Users
      </p>
      <h2 class="font-bold mb-12 text-[35px] leading-10 mt-3 md:text-[52px]">Don't just take our words</h2>

      <!-- Swiper Testimonial Cards -->
      <swiper
        :slides-per-view="1"
        :space-between="30"
        :breakpoints="breakpoints"
        class="w-[85%]"
        loop
        @swiper="onSwiper"
        @slideChange="onSlideChange"
        :autoplay="{ delay: 3000, disableOnInteraction: false }"
      >
        <!-- Testimonial 1 -->
        <swiper-slide>
          <div class="flex flex-col md:flex-row gap-4 items-center text-center rounded-lg">
            <div class="w-[85%]">
              <img
                src="/images/testimonial.png"
                alt="User 1"
                class="rounded-sm mb-4 object-cover"
              />
            </div>
            <div class="text-left h-full flex flex-col justify-between pb-10">
              <div>
                <div class="flex space-x-1 mb-4 text-blue-500">
                  <!-- Star Rating -->
                  <span>⭐</span>
                  <span>⭐</span>
                  <span>⭐</span>
                  <span>⭐</span>
                  <span>⭐</span>
                </div>
                <p class="text-black font-semibold mb-6 text-[16px]">
                  "I appreciate the transparent pricing and the powerful features that come with it. It's been a seamless experience, and the customer support is exceptional!"
                </p>
              </div>
              <div class="flex gap-2">
                <p class="font-bold">Jenny Wilson</p>
                <p class="">New Trader</p>
              </div>
            </div>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="flex flex-col md:flex-row gap-4 items-center text-center rounded-lg">
            <div class="w-[85%]">
              <img
                src="/images/testimonial2.png"
                alt="User 1"
                class="rounded-sm mb-4 object-cover"
              />
            </div>
            <div class="text-left h-full flex flex-col justify-between pb-10">
              <div>
                <div class="flex space-x-1 mb-4 text-blue-500">
                  <!-- Star Rating -->
                  <span>⭐</span>
                  <span>⭐</span>
                  <span>⭐</span>
                  <span>⭐</span>
                  <span>⭐</span>
                </div>
                <p class="text-black font-semibold mb-6 text-[16px]">
                  "The 24/7 monitoring and instant alerts keep me connected to my trades no matter where I am. This software has made trading more convenient and profitable."
                </p>
              </div>
              <div class="flex gap-2">
                <p class="font-bold">Jenny Wilson</p>
                <p class="">New Trader</p>
              </div>
            </div>
          </div>
        </swiper-slide>
       
        
       

        <!-- Additional slides here -->
      </swiper>
    </div>
  </section>
</template>

<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";
import "swiper/css/pagination";

// Import Swiper modules

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    const breakpoints = {
      // When the viewport is ≥ 640px
      640: {
        slidesPerView: 1,
        spaceBetween: 20,
      },
      // When the viewport is ≥ 1024px
      1024: {
        slidesPerView: 2,
        spaceBetween: 30,
      },
    };

    const onSwiper = (swiper) => {
      console.log(swiper);
    };

    const onSlideChange = () => {
      console.log("slide change");
    };

    return {
      breakpoints,
      onSwiper,
      onSlideChange,
    };
  },
  // Register Swiper modules
};
</script>

<style scoped>
/* Add any additional styles you want here */
</style>
