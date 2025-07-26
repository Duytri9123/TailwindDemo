<template>
  <div class="container mx-auto justify-center lg:w-7/8 w-full mb-8 p-2">
    <div class="flex md:flex-row flex-col justify-between lg:items-center lg:mb-8 gap-4">
      <h1
        class="lg:text-2xl md:text-xl text-base text-center whitespace-nowrap font-bold text-gray-800"
      >
        Đội ngũ bác sĩ bệnh viện đa khoa Phương Đông
      </h1>
      <button
        class="cursor-pointer bg-button hover:bg-button text-white font-semibold py-2 px-4 rounded-full text-base flex max-w-40"
      >
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M11 15H7C4.79086 15 3 16.7909 3 19V20"
            stroke="white"
            stroke-width="1.7"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <circle
            cx="11"
            cy="7"
            r="4"
            stroke="white"
            stroke-width="1.7"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <circle
            cx="17.4444"
            cy="16.5556"
            r="3.55556"
            stroke="white"
            stroke-width="1.7"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
          <path
            d="M14.9303 19.0698L13 21.0001"
            stroke="white"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>

        Tìm bác sĩ
      </button>
    </div>
    <div class="w-full grid grid-cols-1 md:grid-cols-2 lg:gap-8 gap-1">
      <div class="items-center rounded-lg justify-center lg:gap-8 gap-4 grid md:grid-cols-2 grid-cols-3">
        <!-- image -->
        <div class="col-span-1 relative cursor-pointer">
          <div class="relative z-20 rounded-b-full p-4 overflow-hidden">
            <img
              src="../Images/NTC.png"
              alt="BS. NGUYÊN TRUNG CHÍNH"
              class="object-contain translate-y-1/9"
            />
          </div>
          <div
            class="absolute rounded-full bg-gradient-mygreen w-full bottom-0 z-0 aspect-square"
          ></div>
        </div>
        <!-- profile -->
        <div class="md:col-span-1 col-span-2 flex justify-center flex-col translate-y-1/9 p-2">
          <h2
            class="xl:text-lg lg:text-base md:text-sm text-2xs font-semibold whitespace-nowrap text-gray-900"
          >
            BS: NGUYỄN TRUNG CHÍNH
          </h2>
          <p class="text-gray-600 xl:text-base lg:text-sm md:text-xs text-[14px]">
            PGS.TS. Bác sĩ Ung bướu - Giám đốc Bệnh viện Đa khoa Phương Đông
          </p>
          <p class="text-gray-700 mt-2 xl:text-base lg:text-sm md:text-xs text-[14px]">
            Kinh nghiệm:
            <span class="font-bold xl:text-base lg:text-sm md:text-xs text-[14px]"
              >20 năm</span
            >
          </p>
          <div class="flex items-center mt-1">
            <span class="text-gray-700 mr-2 xl:text-base lg:text-sm md:text-xs text-[14px]"
              >Xếp hạng:</span
            >
            <div class="flex">
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
            </div>
          </div>
        </div>
      </div>
      <div class="items-center rounded-lg justify-center lg:gap-8 gap-4 grid md:grid-cols-2 grid-cols-3">
        <!-- image -->
        <div class="col-span-1 relative cursor-pointer">
          <div class="relative z-10 rounded-b-full p-4 overflow-hidden">
            <img src="../Images/NHB.png" alt="" class="object-contain translate-y-1/9" />
          </div>
          <div
            class="absolute rounded-full bg-gradient-mygreen w-full bottom-0 z-0 aspect-square"
          ></div>
        </div>
        <!-- profile -->
        <div class="md:col-span-1 col-span-2 flex justify-center flex-col translate-y-1/9 p-2">
          <h2
            class="xl:text-lg lg:text-base md:text-sm text-2xs font-semibold whitespace-nowrap text-gray-900"
          >
            BS: NGUYỄN HUY BẠO
          </h2>
          <p class="text-gray-600 xl:text-base lg:text-sm md:text-xs text-[14px]">
            PGS.TS. Bác sĩ Ung bướu - Phó giám đốc Bệnh viện Đa khoa Phương Đông
          </p>
          <p class="text-gray-700 mt-2 xl:text-base lg:text-sm md:text-xs text-[14px]">
            Kinh nghiệm:
            <span class="font-bold xl:text-base lg:text-sm md:text-xs text-[14px]"
              >20 năm</span
            >
          </p>
          <div class="flex items-center mt-1">
            <span class="text-gray-700 mr-2 xl:text-base lg:text-sm md:text-xs text-[14px]"
              >Xếp hạng:</span
            >
            <div class="flex">
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
            </div>
          </div>
        </div>
      </div>
      <div class="items-center rounded-lg justify-center lg:gap-8 gap-4 grid md:grid-cols-2 grid-cols-3">
        <!-- profile -->
        <div class="md:col-span-1 col-span-2 flex justify-center flex-col translate-y-1/9 p-2">
          <h2
            class="xl:text-lg lg:text-base md:text-sm text-2xs font-semibold whitespace-nowrap text-gray-900"
          >
            BS: TRẦN KINH TRANG
          </h2>
          <p class="text-gray-600 xl:text-base lg:text-sm md:text-xs text-[14px]">
            PGS.TS. Bác sĩ Ung bướu - Phó giám đốc Bệnh viện Đa khoa Phương Đông
          </p>
          <p class="text-gray-700 mt-2 xl:text-base lg:text-sm md:text-xs text-[14px]">
            Kinh nghiệm:
            <span class="font-bold xl:text-base lg:text-sm md:text-xs text-[14px]"
              >20 năm</span
            >
          </p>
          <div class="flex items-center mt-1">
            <span class="text-gray-700 mr-2 xl:text-base lg:text-sm md:text-xs text-[14px]"
              >Xếp hạng:</span
            >
            <div class="flex">
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
            </div>
          </div>
        </div>
        <!-- image -->
        <div class="col-span-1 relative cursor-pointer">
          <div class="relative z-10 rounded-b-full p-4 overflow-hidden">
            <img
              src="../Images/TKT.png"
              alt=""
              class="object-contain translate-y-1/9"
            />
          </div>
          <div
            class="absolute rounded-full bg-gradient-mygreen w-full bottom-0 z-0 aspect-square"
          ></div>
        </div>
      </div>
      <div class="items-center rounded-lg justify-center lg:gap-8 gap-4 grid md:grid-cols-2 grid-cols-3">
        <!-- profile -->
        <div class="md:col-span-1 col-span-2 flex justify-center flex-col translate-y-1/9 p-2">
          <h2
            class="xl:text-lg lg:text-base md:text-sm text-2xs font-semibold whitespace-nowrap text-gray-900"
          >
            DS: NGUYỄN THỊ KIM YẾN
          </h2>
          <p class="text-gray-600 xl:text-base lg:text-sm md:text-xs text-[14px]">
            PGS.TS. Bác sĩ Ung bướu - Phó giám đốc Bệnh viện Đa khoa Phương Đông
          </p>
          <p class="text-gray-700 mt-2 xl:text-base lg:text-sm md:text-xs text-[14px]">
            Kinh nghiệm:
            <span class="font-bold xl:text-base lg:text-sm md:text-xs text-[14px]"
              >20 năm</span
            >
          </p>
          <div class="flex items-center mt-1">
            <span class="text-gray-700 mr-2 xl:text-base lg:text-sm md:text-xs text-[14px]"
              >Xếp hạng:</span
            >
            <div class="flex">
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
              <svg class="w-5 h-5 text-yellow-400 fill-current" viewBox="0 0 24 24">
                <path
                  d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2 9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                />
              </svg>
            </div>
          </div>
        </div>
        <!-- image -->
        <div class="col-span-1 relative cursor-pointer">
          <div class="relative z-20 rounded-b-full p-4 overflow-hidden">
            <img
              src="../Images/NTKY.png"
              alt=""
              class="object-contain translate-y-1/9"
            />
          </div>
          <div
            class="absolute rounded-full bg-gradient-mygreen w-full bottom-0 z-0 aspect-square"
          ></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
