<template>
  <div
    class="flex flex-col relative w-full px-4 lg:mt-44 mt-10 bg-white lg:gap-8 gap-4 space-y-8 items-center justify-center"
  >
    <div class="lg:w-5/7 flex lg:flex-row flex-col justify-between lg:gap-8 gap-6">
      <h1 class="text-xl md:text-4xl lg:text-4xl font-medium whitespace-nowrap">
        Hình ảnh về cơ sở vật chất, trang thiết bị
      </h1>
      <!-- Nút điều hướng -->
      <div class="flex gap-6 z-10 mx-4 lg:justify-end justify-center">
        <button
          class="cursor-pointer swiper-button-prev-custom text-2xl w-10 h-10 text-white rounded-full flex items-center justify-center bg-button hover:bg-button drop-shadow-2xl/25"
        >
          <svg
            width="10"
            height="16"
            viewBox="0 0 10 16"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M8.5 15L1.5 8L8.5 1"
              stroke="white"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </button>
        <button
          class="cursor-pointer swiper-button-next-custom text-2xl w-10 h-10 text-white rounded-full flex items-center justify-center bg-button hover:bg-button drop-shadow-2xl/25"
        >
          <svg
            width="10"
            height="16"
            viewBox="0 0 10 16"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M1.5 15L8.5 8L1.5 1"
              stroke="white"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </button>
      </div>
    </div>

    <swiper
      :modules="[Navigation]"
      :loop="true"
      :autoplay="200"
      :space-between="25"
      :slides-per-view="2"
      :navigation="customNavigation"
      :breakpoints="breakpoints"
      class="w-full"
    >
      <swiper-slide
        v-for="(image, index) in images"
        :key="index"
        @click="openZoom(image)"
        class="rounded-t-2xl rounded-br-2xl overflow-hidden cursor-pointer"
      >
        <div
          class="relative w-full aspect-[2/3] overflow-hidden rounded-br-2xl xl:rounded-t-[var(--g-40)] xl:rounded-br-[var(--g-40)]"
        >
          <img :src="image" class="w-full aspect-[2/3] object-cover" />
        </div>
      </swiper-slide>
    </swiper>
    <div
      v-if="showZoom"
      class="fixed inset-0 bg-gray-700/60 flex items-center justify-center z-[999]"
      @click.self="showZoom = false"
    >
      <swiper :initial-slide="zoomIndex" :slides-per-view="1" :loop="true" class="w-full">
        <swiper-slide
          v-for="(image, index) in images"
          :key="index"
          @click.self="showZoom = false"
          class="flex items-center justify-center"
        >
          <div>
            <img
              :src="image"
              class="max-h-[70vh] object-contain rounded-xl mx-auto my-auto"
            />
          </div>
        </swiper-slide>
      </swiper>
    </div>
  </div>
</template>

<script setup>
import { Swiper, SwiperSlide } from "swiper/vue";
import { Navigation } from "swiper/modules";
import { ref } from "vue";

import "swiper/css";
import "swiper/css/navigation";
const zoomImage = ref("");
const showZoom = ref(false);

function openZoom(imgUrl) {
  zoomImage.value = imgUrl;
  showZoom.value = true;
}
const customNavigation = {
  nextEl: ".swiper-button-next-custom",
  prevEl: ".swiper-button-prev-custom",
};
const breakpoints = {
  640: { slidesPerView: 2 },
  768: { slidesPerView: 3 },
  1024: { slidesPerView: 4 },
  1280: { slidesPerView: 5 },
  1563: { slidesPerView: 6 },
};
const baseImages = [
  new URL("@/Images/stomatological-1.jpg", import.meta.url).href,
  new URL("@/Images/modern-surgical.jpg", import.meta.url).href,
  new URL("@/Images/dental3.jpg", import.meta.url).href,
  new URL("@/Images/rendering4.jpg", import.meta.url).href,
  new URL("@/Images/modern-5.jpg", import.meta.url).href,
  new URL("@/Images/newest-6.jpg", import.meta.url).href,
];

const images = [...baseImages, ...baseImages.slice(0, 2)];
</script>
