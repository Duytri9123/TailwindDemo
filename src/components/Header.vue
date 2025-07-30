<template>
  <header
    :class="[
      'fixed top-0 left-0 right-0 z-50 bg-white shadow-lg transition-transform duration-500',
      isHidden ? '-translate-y-full' : 'translate-y-0',
    ]"
    class="w-screen flex justify-center items-center px-4 md:px-6 lg:px-10 xl:px-16 py-2 md:py-2.5 h-14 lg:h-16"
  >
    <div
      class="flex justify-between items-center lg:h-10 h-8 2xl:gap-24 xl:gap-12 lg:gap-8 w-full xl:w-auto"
    >
      <!-- LOGO -->
      <a href="#" class="h-full w-auto container flex items-center">
        <img src="../Images/logo.png" alt="logo" class="h-full object-contain" />
      </a>
      <!-- navigate -->
      <nav class="hidden lg:flex items-center gap-x-4 xl:gap-x-8 2xl:gap-x-14">
        <a
          v-for="(item, index) in navtive"
          :key="index"
          href="#"
          class="font-roboto font-medium text-gray-800 hover:text-blue-600 hover:underline text-sm md:text-base xl:text-lg whitespace-nowrap"
          >{{ item }}</a
        >
      </nav>
      <!-- Hotline -->
      <a
        href="tel:19001806"
        class="hidden lg:flex items-center gap-2 rounded-full px-4 h-10 bg-button text-white font-bold drop-shadow-md/25 text-xs md:text-sm xl:text-base hover:bg-button whitespace-nowrap"
      >
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            fill-rule="evenodd"
            clip-rule="evenodd"
            d="M18.965 16.61L17.792 15.437C17.206 14.851 16.256 14.851 15.671 15.437L14.749 16.359C14.543 16.565 14.231 16.634 13.965 16.517C12.629 15.932 11.309 15.045 10.132 13.868C8.95999 12.696 8.07599 11.382 7.48999 10.051C7.36799 9.77597 7.43899 9.45297 7.65199 9.23997L8.47799 8.41397C9.14899 7.74297 9.14899 6.79397 8.56299 6.20797L7.38999 5.03497C6.60899 4.25397 5.34299 4.25397 4.56199 5.03497L3.90999 5.68597C3.16899 6.42697 2.85999 7.49597 3.05999 8.55597C3.55399 11.169 5.07199 14.03 7.52099 16.479C9.96999 18.928 12.831 20.446 15.444 20.94C16.504 21.14 17.573 20.831 18.314 20.09L18.965 19.439C19.746 18.658 19.746 17.392 18.965 16.61Z"
            fill="white"
            stroke="white"
            stroke-width="0.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M13 6.99109C14.031 6.97709 15.067 7.35909 15.854 8.14609"
            stroke="white"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M18.682 5.31787C17.113 3.74887 15.056 2.96387 13 2.96387"
            stroke="white"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M17.009 11C17.023 9.969 16.641 8.933 15.854 8.146"
            stroke="white"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M18.682 5.31787C20.251 6.88687 21.036 8.94387 21.036 10.9999"
            stroke="white"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
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
        @click.self="closeModal"
        class="bg-gray-200/50 h-screen w-screen fixed top-0 left-0 lg:hidden"
      >
        <div
          class="lg:hidden bg-white h-screen flex md:w-1/2 w-3/4 fixed top-0 right-0 flex-col shadow-lg"
        >
          <div class="flex justify-between lg:h-16 h-14 items-center md:px-4 mb-0.5 px-2">
            <a href="#" class="lg:h-10 h-8">
              <img src="../Images/logo.png" alt="logo" class="object-fit h-full" />
            </a>
            <button
              type="button"
              @click="closeModal"
              class="text-gray-700 hover:text-blue-600 focus:outline-none mr-4"
            >
              <svg
                class="w-5 h-5"
                fill="none"
                stroke="currentColor"
                viewBox="0 0 24 24"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M6 18L18 6M6 6l12 12"
                ></path>
              </svg>
            </button>
          </div>

          <nav class="relative flex flex-col pb-4 bg-blue-100/30 h-full">
            <a
              v-for="(item, index) in navtive"
              :key="index"
              href="#"
              @click="isModal = false"
              class="block text-gray-700 hover:text-blue-600 hover:bg-amber-100 font-medium py-4 px-4 w-full shadow-[0_2px_0_rgba(0,0,0,0.2)] transform hover:translate-y-1 transition duration-300 border-t-2 border-gray-200"
              >{{ item }}</a
            >
          </nav>
        </div>
      </div>
    </div>
  </header>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from "vue";

const navtive = ref([
  "Ưu đãi",
  "Dịch vụ",
  "Giới thiệu",
  "Đội ngũ bác sĩ",
  "Bảng giá",
  "Thư viện",
  "Liên hệ",
]);
const isModal = ref(false);
const isHidden = ref(false);
let lastScrollY = window.scrollY;

const handOpenModal = () => {
  isModal.value = true;
  document.body.classList.add("overflow-hidden");
};

const closeModal = () => {
  isModal.value = false;
  document.body.classList.remove("overflow-hidden");
};

const handleScroll = () => {
  const currentY = window.scrollY;

  if (currentY > lastScrollY && currentY > 50) {
    isHidden.value = true;
  } else {
    isHidden.value = false; // cuộn lên trên hoặc không cuộn
  }

  lastScrollY = currentY;
};

onMounted(() => {
  window.addEventListener("scroll", handleScroll);
});
onUnmounted(() => {
  window.removeEventListener("scroll", handleScroll);
});
</script>

<style lang="scss" scoped></style>
