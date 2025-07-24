<template>
  <nav
    class="w-screen h-auto container z-50 flex lg:flex-row flex-col lg:gap-10 gap-6"
  >
    <div class="w-full lg:w-1/4 h-1/2 lg:gap-10 md:gap-4 gap-2 flex flex-col">
      <span
        class="2xl:text-4xl xl:text-3xl lg:text-2xl text-xl font-semibold text-gray-900 leading-11 font-roboto text-nowrap"
        >Chương trình ưu đãi:</span
      >
      <span
        class="max-w-3/4 lg:w-full text-gray-700 2xl:text-base/normal lg:text-sm/normal text-xs/normal"
      >
        Lorem ipsum dolor sit amet, consectetur adipiscing elit lis iaculis ac felis
        porta. Vulputate tellus sapien pat sit ipsum molestie pharetran da volutpat
        semper.
      </span>
      <div class="inline-block lg:space-x-5 space-x-3">
        <button
          class="lg:w-10 md:w-8 aspect-square rounded-full text-white gap-3 md:gap-6 lg:gap-10 lg:px-3 px-2 bg-linear-to-t from-[var(--color-orange-dark)] to-[var(--color-orange-light)] hover:to-30% drop-shadow-2xl/25"
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
          class="lg:w-10 md:w-8 aspect-square rounded-full text-white gap-3 md:gap-6 lg:gap-10 lg:px-3 px-2 bg-linear-to-t from-[var(--color-orange-dark)] to-[var(--color-orange-light)] hover:to-30% drop-shadow-2xl/25"
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

    <div class="flex gap-5  overflow-hidden items-stretch">
      <div
        class="relative aspect-[2/3] max-h-2/3  rounded-tl-[20px] rounded-tr-[20px] bg-white"
      >
        <!-- img  -->
        <img
          src="../Images/human-fetus.jpg"
          alt=""
          class="w-full object-cover 2xl:rounded-tl-[40px] lg:rounded-tl-[32px] md:rounded-tl-[24px]"
        />
        <!-- title -->
        <div
          class="transform -translate-y-12 w-fit bottom-0 xl:rounded-tl-[40px] xl:rounded-tr-[40px] xl:rounded-br-[40px] bg-gradient-to-r from-[#50C577] to-[#2DBEFC] xl:px-4 xl:py-6 xl:gap-4 md:px-3 md:py-5 md:gap-3 px-2 py-4 gap-2 lg:rounded-tl-[32px] lg:rounded-tr-[32px] lg:rounded-br-[32px] rounded-tl-[24px] rounded-tr-[24px] rounded-br-[24px]"
        >
          <div class="flex flex-col justify-center items-center text-center">
            <span
              class="font-arima font-medium text-white text-lg sm:text-xl lg:text-2xl leading-tight text-nowrap"
              >Ưu đãi 50%</span
            >
            <span
              class="font-roboto font-medium text-white text-sm sm:text-base lg:text-lg text-nowrap"
              >Gói khám thai tổng quát</span
            >
            <span
              class="hidden lg:block font-roboto font-normal text-white text-xs sm:text-sm leading-snug"
              >Lorem ipsum dolor sit amet tarancebe consectetur adipiscing elit
              turpis.</span
            >
            <button
              class="mt-2 px-4 py-2 sm:px-6 sm:py-2.5 bg-gradient-to-t from-[var(--color-orange-light)] to-[var(--color-orange-dark)] drop-shadow-2xl/20 hover:to-35% rounded-full text-white text-xs sm:text-sm lg:text-base font-semibold text-nowrap"
            >
              Đăng ký nhận ưu đãi
            </button>
          </div>
        </div>
      </div>
      <div
        class="relative aspect-[2/3] max-h-2/3 container rounded-tl-[20px] rounded-tr-[20px] bg-white"
      >
        <!-- img  -->
        <img
          src="../Images/human-fetus.jpg"
          alt=""
          class="w-full object-cover 2xl:rounded-tl-[40px] lg:rounded-tl-[32px] md:rounded-tl-[24px]"
        />
        <!-- title -->
        <div
          class="transform -translate-y-12 w-fit bottom-0 xl:rounded-tl-[40px] xl:rounded-tr-[40px] xl:rounded-br-[40px] bg-white xl:px-4 drop-shadow-sm/10 xl:py-6 xl:gap-4 md:px-3 md:py-5 md:gap-3 px-2 py-4 gap-2 lg:rounded-tl-[32px] lg:rounded-tr-[32px] lg:rounded-br-[32px] rounded-tl-[24px] rounded-tr-[24px] rounded-br-[24px]"
        >
          <div class="flex flex-col justify-center items-center text-center">
            <span
              class="font-arima font-medium text-gray-800 text-lg sm:text-xl lg:text-2xl leading-tight text-nowrap"
              >Ưu đãi 50%</span
            >
            <span
              class="font-roboto font-medium text-gray-800 text-sm sm:text-base lg:text-lg text-nowrap"
              >Gói khám thai tổng quát</span
            >
            <span
              class="hidden lg:block font-roboto font-normal text-gray-800 text-xs sm:text-sm leading-snug"
              >Lorem ipsum dolor sit amet tarancebe consectetur adipiscing elit
              turpis.</span
            >
            <button
              class="mt-2 px-4 py-2 sm:px-6 sm:py-2.5 border border-[var(--color-orange-light)] text-[var(--color-orange-light)] bg-gradient-to-t hover:from-[var(--color-orange-light)] hover:to-[var(--color-orange-dark)] drop-shadow-2xl/20 hover:to-35% rounded-full text-xs sm:text-sm lg:text-base font-semibold text-nowrap"
            >
              Đăng ký nhận ưu đãi
            </button>
          </div>
        </div>
      </div>
      <div
        class="relative aspect-[2/3] max-h-2/3 container rounded-tl-[20px] rounded-tr-[20px] bg-white"
      >
        <!-- img  -->
        <img
          src="../Images/human-fetus.jpg"
          alt=""
          class="w-full object-cover 2xl:rounded-tl-[40px] lg:rounded-tl-[32px] md:rounded-tl-[24px]"
        />
        <!-- title -->
        <div
          class="transform -translate-y-12 w-fit bottom-0 xl:rounded-tl-[40px] xl:rounded-tr-[40px] xl:rounded-br-[40px] bg-white xl:px-4 drop-shadow-sm/10 xl:py-6 xl:gap-4 md:px-3 md:py-5 md:gap-3 px-2 py-4 gap-2 lg:rounded-tl-[32px] lg:rounded-tr-[32px] lg:rounded-br-[32px] rounded-tl-[24px] rounded-tr-[24px] rounded-br-[24px]"
        >
          <div class="flex flex-col justify-center items-center text-center">
            <span
              class="font-arima font-medium text-gray-800 text-lg sm:text-xl lg:text-2xl leading-tight text-nowrap"
              >Ưu đãi 50%</span
            >
            <span
              class="font-roboto font-medium text-gray-800 text-sm sm:text-base lg:text-lg text-nowrap"
              >Gói khám thai tổng quát</span
            >
            <span
              class="hidden lg:block font-roboto font-normal text-gray-800 text-xs sm:text-sm leading-snug"
              >Lorem ipsum dolor sit amet tarancebe consectetur adipiscing elit
              turpis.</span
            >
            <button
              class="mt-2 px-4 py-2 sm:px-6 sm:py-2.5 border border-[var(--color-orange-light)] text-[var(--color-orange-light)] bg-gradient-to-t hover:from-[var(--color-orange-light)] hover:to-[var(--color-orange-dark)] drop-shadow-2xl/20 hover:to-35% rounded-full text-xs sm:text-sm lg:text-base font-semibold text-nowrap"
            >
              Đăng ký nhận ưu đãi
            </button>
          </div>
        </div>
      </div>
      <div
        class="relative aspect-[2/3] max-h-2/3 container rounded-tl-[20px] rounded-tr-[20px] bg-white"
      >
        <!-- img  -->
        <img
          src="../Images/human-fetus.jpg"
          alt=""
          class="w-full object-cover 2xl:rounded-tl-[40px] lg:rounded-tl-[32px] md:rounded-tl-[24px]"
        />
        <!-- title -->
        <div
          class="transform -translate-y-12 w-fit bottom-0 xl:rounded-tl-[40px] xl:rounded-tr-[40px] xl:rounded-br-[40px] bg-white xl:px-4 drop-shadow-sm/10 xl:py-6 xl:gap-4 md:px-3 md:py-5 md:gap-3 px-2 py-4 gap-2 lg:rounded-tl-[32px] lg:rounded-tr-[32px] lg:rounded-br-[32px] rounded-tl-[24px] rounded-tr-[24px] rounded-br-[24px]"
        >
          <div class="flex flex-col justify-center items-center text-center">
            <span
              class="font-arima font-medium text-gray-800 text-lg sm:text-xl lg:text-2xl leading-tight text-nowrap"
              >Ưu đãi 50%</span
            >
            <span
              class="font-roboto font-medium text-gray-800 text-sm sm:text-base lg:text-lg text-nowrap"
              >Gói khám thai tổng quát</span
            >
            <span
              class="hidden lg:block font-roboto font-normal text-gray-800 text-xs sm:text-sm leading-snug"
              >Lorem ipsum dolor sit amet tarancebe consectetur adipiscing elit
              turpis.</span
            >
            <button
              class="mt-2 px-4 py-2 sm:px-6 sm:py-2.5 border border-[var(--color-orange-light)] text-[var(--color-orange-light)] bg-gradient-to-t hover:from-[var(--color-orange-light)] hover:to-[var(--color-orange-dark)] drop-shadow-2xl/20 hover:to-35% rounded-full text-xs sm:text-sm lg:text-base font-semibold text-nowrap"
            >
              Đăng ký nhận ưu đãi
            </button>
          </div>
        </div>
      </div>
      <div
        class="relative aspect-[2/3] max-h-2/3 container rounded-tl-[20px] rounded-tr-[20px] bg-white"
      >
        <!-- img  -->
        <img
          src="../Images/human-fetus.jpg"
          alt=""
          class="w-full object-cover 2xl:rounded-tl-[40px] lg:rounded-tl-[32px] md:rounded-tl-[24px]"
        />
        <!-- title -->
        <div
          class="transform -translate-y-12 w-fit bottom-0 xl:rounded-tl-[40px] xl:rounded-tr-[40px] xl:rounded-br-[40px] bg-white xl:px-4 drop-shadow-sm/10 xl:py-6 xl:gap-4 md:px-3 md:py-5 md:gap-3 px-2 py-4 gap-2 lg:rounded-tl-[32px] lg:rounded-tr-[32px] lg:rounded-br-[32px] rounded-tl-[24px] rounded-tr-[24px] rounded-br-[24px]"
        >
          <div class="flex flex-col justify-center items-center text-center">
            <span
              class="font-arima font-medium text-gray-800 text-lg sm:text-xl lg:text-2xl leading-tight text-nowrap"
              >Ưu đãi 50%</span
            >
            <span
              class="font-roboto font-medium text-gray-800 text-sm sm:text-base lg:text-lg text-nowrap"
              >Gói khám thai tổng quát</span
            >
            <span
              class="hidden lg:block font-roboto font-normal text-gray-800 text-xs sm:text-sm leading-snug"
              >Lorem ipsum dolor sit amet tarancebe consectetur adipiscing elit
              turpis.</span
            >
            <button
              class="mt-2 px-4 py-2 sm:px-6 sm:py-2.5 border border-[var(--color-orange-light)] text-[var(--color-orange-light)] bg-gradient-to-t hover:from-[var(--color-orange-light)] hover:to-[var(--color-orange-dark)] drop-shadow-2xl/20 hover:to-35% rounded-full text-xs sm:text-sm lg:text-base font-semibold text-nowrap"
            >
              Đăng ký nhận ưu đãi
            </button>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref } from "vue";
</script>

<style lang="scss" scoped></style>
