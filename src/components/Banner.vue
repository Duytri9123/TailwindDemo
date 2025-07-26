<template>
  <nav class="w-screen h-auto container z-50 flex lg:flex-row flex-col lg:gap-10 gap-4">
    <div class="w-full lg:w-1/4 flex flex-col gap-4">
      <span
        class="2xl:text-4xl xl:text-3xl lg:text-2xl text-xl font-semibold text-gray-900 font-roboto text-nowrap"
      >
        Chương trình ưu đãi:
      </span>
      <span class="text-gray-700 2xl:text-base lg:text-sm text-xs leading-relaxed">
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Iaculis ac felis porta.
        Vulputate tellus sapien pat sit ipsum molestie pharetra da volutpat semper.
      </span>
      <div class="inline-flex space-x-4">
        <button
          @click="swiper?.slidePrev()"
          class="cursor-pointer w-10 aspect-square rounded-full text-white bg-button hover:bg-button drop-shadow-lg flex items-center justify-center"
        >
          <svg
            class="w-5 h-5 transform rotate-180"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            viewBox="0 0 24 24"
          >
            <path stroke-linecap="round" stroke-linejoin="round" d="M9 5l7 7-7 7" />
          </svg>
        </button>
        <button
          @click="swiper?.slideNext()"
          class="cursor-pointer w-10 aspect-square rounded-full text-white bg-button hover:bg-button drop-shadow-lg flex items-center justify-center"
        >
          <svg
            class="w-5 h-5"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            viewBox="0 0 24 24"
          >
            <path stroke-linecap="round" stroke-linejoin="round" d="M9 5l7 7-7 7" />
          </svg>
        </button>
      </div>
    </div>

    <div class="w-full lg:w-3/4">
      <Swiper
        :slides-per-view="2.5"
        :autoplay="300"
        :space-between="20"
        :loop="true"
        :breakpoints="{
          640: { slidesPerView: 3 },
          768: { slidesPerView: 3 },
          1024: { slidesPerView: 3 },
          1280: { slidesPerView: 4 },
        }"
        @swiper="onSwiper"
      >
        <SwiperSlide v-for="(item, index) in 5" :key="index" @click="activeIndex = index">
          <div class="cursor-pointer relative aspect-[2/3] rounded-t-2xl">
            <!-- Ảnh -->
            <img
              src="../Images/human-fetus.jpg"
              alt=""
              class="w-full object-cover 2xl:rounded-tl-[40px] lg:rounded-tl-4xl md:rounded-tl-3xl"
            />

            <!-- Nội dung -->
            <div
              class="group cursor-pointer w-full transform -translate-y-12 mx-auto bg-white hover:bg-[linear-gradient(to_right,#50C577,#2DBEFC)] rounded-tl-3xl rounded-tr-3xl rounded-br-3xl px-4 py-4 shadow-md/5 transition-colors duration-300"
            >
              <div class="flex flex-col justify-center items-center text-center">
                <span
                  class="font-arima font-medium text-gray-800 group-hover:text-white text-lg sm:text-xl lg:text-2xl leading-tight text-nowrap transition-colors duration-300"
                >
                  Ưu đãi 50%
                </span>
                <span
                  class="font-roboto font-medium text-gray-800 group-hover:text-white text-sm sm:text-base lg:text-lg text-nowrap transition-colors duration-300"
                >
                  Gói khám thai tổng quát
                </span>
                <span
                  class="font-roboto font-normal text-gray-800 group-hover:text-white text-xs sm:text-sm leading-snug transition-colors duration-300"
                >
                  Lorem ipsum dolor sit amet tarancebe consectetur adipiscing elit turpis.
                </span>

                <button
                  class="mt-2 px-4 py-2 sm:px-6 sm:py-2.5 rounded-full text-xs sm:text-sm lg:text-base font-semibold text-nowrap transition-all duration-300 border border-[var(--color-orange-light)] text-[var(--color-orange-light)] bg-white group-hover:bg-[linear-gradient(to_bottom,#FFB469,#E57709)] group-hover:text-white"
                >
                  Đăng ký nhận ưu đãi
                </button>
              </div>
            </div>
          </div>
        </SwiperSlide>
      </Swiper>
    </div>
  </nav>
</template>

<script setup>
import { ref } from "vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";

const swiper = ref(null);

const onSwiper = (s) => {
  swiper.value = s;
};
</script>

<style scoped lang="scss"></style>
