<template>
  <header class="bg-white shadow-sm w-full h-16 px-2 py-2.5 gap-2.5 relative z-50">
    <div class="container flex justify-between items-center mx-auto h-10">
      <!-- LOGO -->
      <a href="#" class="h-full">
        <img src="../Images/logo.png" alt="logo" class="h-full" />
      </a>
      <!-- navigate -->
      <nav
        class="hidden lg:flex flex-row max-w-fit h-fit xl:gap-14 lg:gap-8 items-center"
      >
        <a
          href="#"
          class="text-gray-700 hover:text-blue-600 font-roboto font-medium text-[18px] leading-6"
          >Trang chủ</a
        >
        <a
          href="#"
          class="text-gray-700 hover:text-blue-600 font-roboto font-medium text-[18px] leading-6"
          >Giới thiệu</a
        >
        <a
          href="#"
          class="text-gray-700 hover:text-blue-600 font-roboto font-medium text-[18px] leading-6"
          >Sản phẩm</a
        >
        <a
          href="#"
          class="text-gray-700 hover:text-blue-600 font-roboto font-medium text-[18px] leading-6"
          >Dịch vụ</a
        >
        <a
          href="#"
          class="text-gray-700 hover:text-blue-600 font-roboto font-medium text-[18px] leading-6"
          >Tin tức</a
        >
        <a
          href="#"
          class="text-gray-700 hover:text-blue-600 font-roboto font-medium text-[18px] leading-6"
          >Liên hệ</a
        >
      </nav>
      <!-- Hotline -->
      <a
        href="tel:19001806"
        class="hidden lg:flex flex-row items-center h-full rounded-[40px] px-4 pr-6 gap-2 text-white font-bold"
        style="background: linear-gradient(to right, #ffb469, #e57709)"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-5 w-5"
          viewBox="0 0 20 20"
          fill="currentColor"
        >
          <path
            d="M2 3a1 1 0 011-1h2.153a1 1 0 01.986.836l.74 4.435a1 1 0 01-.54 1.06l-1.548.774a11.037 11.037 0 006.105 6.105l.774-1.548a1 1 0 011.06-.54l4.435.74a1 1 0 01.836.986V17a1 1 0 01-1 1h-2C7.82 18 2 12.18 2 5V3z"
          />
        </svg>
        <span>Hotline: 1900 1806</span>
      </a>

      <!--icon bar -->
      <button
        type="button"
        @click="handOpenModal"
        class="lg:hidden text-gray-700 hover:text-blue-600 focus:outline-none"
      >
        <svg
          class="w-7 h-7"
          fill="none"
          stroke="currentColor"
          viewBox="0 0 24 24"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M4 6h16M4 12h16m-7 6h7"
          ></path>
        </svg>
      </button>
      <!-- nagative mobile -->
      <div
        v-show="isModal"
        class="lg:hidden bg-white py-2 shadow-md md:w-1/4 w-1/2 absolute right-0 top-full z-50 flex flex-col p-4"
      >
        <nav class="flex flex-col items-center space-y-2 pb-4">
          <a
            href="#"
            @click="isModal = false"
            class="block text-gray-700 hover:text-blue-600 font-medium py-2 px-4 w-full text-center"
            >Trang chủ</a
          >
          <a
            href="#"
            @click="isModal = false"
            class="block text-gray-700 hover:text-blue-600 font-medium py-2 px-4 w-full text-center"
            >Giới thiệu</a
          >
          <a
            href="#"
            @click="isModal = false"
            class="block text-gray-700 hover:text-blue-600 font-medium py-2 px-4 w-full text-center"
            >Sản phẩm</a
          >
          <a
            href="#"
            @click="isModal = false"
            class="block text-gray-700 hover:text-blue-600 font-medium py-2 px-4 w-full text-center"
            >Dịch vụ</a
          >
          <a
            href="#"
            @click="isModal = false"
            class="block text-gray-700 hover:text-blue-600 font-medium py-2 px-4 w-full text-center"
            >Tin tức</a
          >
          <a
            href="#"
            @click="isModal = false"
            class="block text-gray-700 hover:text-blue-600 font-medium py-2 px-4 w-full text-center"
            >Liên hệ</a
          >
        </nav>
      </div>
    </div>
  </header>
</template>

<script setup>
import { ref } from "vue";

const isModal = ref(false);

const handOpenModal = () => {
  console.log("hello");
  isModal.value = !isModal.value;
};
</script>

<style lang="scss" scoped></style>
