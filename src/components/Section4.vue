<template>
  <div class="relative w-full px-4 md:py-8 bg-white">
    <div class="flex flex-row justify-evenly">
      <h2 class="text-center text-lg md:text-2xl font-semibold mb-6 whitespace-nowrap">
        Hình ảnh về cơ sở vật chất, trang thiết bị
      </h2>
      <!-- Nút điều hướng -->
      <div class="flex gap-2 z-10 mx-4">
        <button
          class="swiper-button-prev-custom w-8 h-8 text-white rounded-full flex items-center justify-center bg-linear-to-t from-[var(--color-orange-dark)] to-[var(--color-orange-light)] hover:to-30% drop-shadow-2xl/25"
        >
          ‹
        </button>
        <button
          class="swiper-button-next-custom w-8 h-8 text-white rounded-full flex items-center justify-center bg-linear-to-t from-[var(--color-orange-dark)] to-[var(--color-orange-light)] hover:to-30% drop-shadow-2xl/25"
        >
          ›
        </button>
      </div>
    </div>

    <swiper
      :modules="[Navigation]"
      :loop="true"
      :space-between="20"
      :slides-per-view="2"
      :navigation="customNavigation"
      :breakpoints="breakpoints"
      class="w-full"
    >
      <swiper-slide
        v-for="(image, index) in images"
        :key="index"
        class="rounded-t-2xl rounded-br-2xl overflow-hidden"
      >
        <img
          :src="image"
          class="w-full md:h-80 h-60 object-cover rounded-t-2xl rounded-br-2xl"
        />
      </swiper-slide>
    </swiper>
  </div>
</template>

<script setup>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Navigation } from "swiper/modules";

import "swiper/css";
import "swiper/css/navigation";

const customNavigation = {
  nextEl: ".swiper-button-next-custom",
  prevEl: ".swiper-button-prev-custom",
};
const breakpoints = {
  640: { slidesPerView: 3 },
  768: { slidesPerView: 4 },
  1024: { slidesPerView: 5 },
  1280: { slidesPerView: 6 },
};
const baseImages = [
  new URL("@/Images/modern-5.jpg", import.meta.url).href,
  new URL("@/Images/modern-surgical.jpg", import.meta.url).href,
  new URL("@/Images/h1.jpg", import.meta.url).href,
  new URL("@/Images/mother-newborn.jpg", import.meta.url).href,
  new URL("@/Images/stomatological-1.jpg", import.meta.url).href,
  new URL("@/Images/human-fetus.jpg", import.meta.url).href,
];

const images = [...baseImages, ...baseImages.slice(0, 2)];
</script>
