<template>
  <nav
    class="w-screen z-50 flex lg:flex-row flex-col xl:gap-4 lg:gap-10 gap-6 transform translate-x-0 lg:translate-x-1/8 px-2"
  >
    <div class="w-full lg:w-1/4 flex flex-col lg:gap-12 gap-4 mx-auto">
      <div
        class="w-full lg:w-full lg:gap-4 gap-2 flex flex-col items-center lg:items-start justify-center lg:justify-start m-2 "
      >
        <h1
          class="xl:text-[36px] lg:text-3xl text-xl font-medium text-black font-roboto text-nowrap lg:gap-4 gap-2"
        >
          Chương trình ưu đãi:
        </h1>

        <span class="text-gray-600 text-sm sm:text-[16px] tracking-[0.5px] lg:px-0 px-4">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit lis iaculis ac felis
          porta. Vulputate tellus sapien pat sit ipsum molestie pharetran da volutpat
          semper.
        </span>
      </div>

      <div class="inline-flex justify-center lg:justify-start px-2 gap-4">
        <button
          @click="swiper?.slidePrev()"
          class="cursor-pointer lg:w-10 w-8 gap-2 aspect-square rounded-full text-white bg-button hover:bg-button drop-shadow-lg flex items-center justify-center"
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
          @click="swiper?.slideNext()"
          class="cursor-pointer lg:w-10 w-8 gap-2 aspect-square rounded-full text-white bg-button hover:bg-button drop-shadow-lg flex items-center justify-center"
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

    <div class="w-full lg:w-3/4">
      <Swiper
        :slides-per-view="2"
        :autoplay="200"
        :space-between="25"
        :loop="true"
        :breakpoints="{
          640: { slidesPerView: 3 },
          768: { slidesPerView: 3 },
          1024: { slidesPerView: 3 },
          1280: { slidesPerView: 4 },
          1536: { slidesPerView: 4 },
        }"
        @swiper="onSwiper"
      >
        <SwiperSlide v-for="(item, index) in 5" :key="index" @click="activeIndex = index">
          <div
            class="cursor-pointer relative aspect-[2/3] overflow-clip rounded-tl-[40px] rounded-br-[40px]"
          >
            <!-- Ảnh -->
            <div class="w-full scale-100 md:-translate-y-11 -translate-y-7 transition-all duration-500 xl:rounded-tl-[40px] lg:rounded-tl-4xl md:rounded-tl-3xl">
              <img
                src="../Images/human-fetus.jpg"
                alt=""
                class="w-full h-full object-cover"
              />

            </div>

            <!-- Nội dung -->
            <div
              class="group cursor-pointer w-full transform 2xl:-translate-y-1/2 lg:-translate-y-1/3 md:-translate-y-1/2 -translate-y-1/4 mx-auto bg-white hover:bg-[linear-gradient(to_right,#50C577,#2DBEFC)] lg:rounded-tl-[40px] lg:rounded-tr-[40px] lg:rounded-br-[40px] rounded-tl-4xl rounded-tr-4xl rounded-br-4xl md:px-4 px-2 py-6 md:gap-4 gap-2 shadow-md/5"
            >
              <div class="flex flex-col justify-center items-center text-center gap-4">
                <div class="flex flex-col items-center gap-2">
                  <span
                    class="font-arima font-medium bg-clip-text text-transparent bg-gradient-to-r from-[#50C577] to-[#2DBEFC] group-hover:text-white text-2xl md:text-3xl lg:text-[32px] leading-tight text-nowrap"
                  >
                    Ưu đãi 50%
                  </span>
                  <span
                    class="font-roboto font-medium text-gray-800 group-hover:text-white text-sm md:text-[20px] lg:text-lg 2xl:text-[22px] text-nowrap"
                  >
                    Gói khám thai tổng quát
                  </span>
                  <span
                    class="font-roboto font-normal md:tracking-[0.5px] text-gray-600 group-hover:text-white text-xs md:text-base"
                  >
                    Lorem ipsum dolor sit amet tarancebe consectetur adipiscing elit
                    turpis.
                  </span>
                </div>

                <a
                   href="tel:123456"
                  class="w-full sm:py-2.5 gap-2 rounded-full font-semibold text-nowrap border border-[var(--color-orange-light)] bg-white group-hover:bg-[linear-gradient(to_bottom,#FFB469,#E57709)] group-hover:text-white"
                >
                  <span
                    class="bg-button bg-clip-text text-transparent tracking-[0.5px] font-roboto font-semibold group-hover:text-white text-xs md:text-base lg:lg text-nowrap"
                    >Đăng ký nhận ưu đãi</span
                  >
                </a>
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
