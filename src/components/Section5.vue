<template>
  <div class="flex justify-center items-center mb-16 lg:p-4 pt-10">
    <div class="w-8/9 lg:w-6/8 mx-auto">
      <div class="flex lg:flex-row flex-col justify-between gap-4">
        <h1 class="text-base md:text-3xl lg:text-4xl font-medium whitespace-nowrap">
          Đội ngũ bác sĩ bệnh viện đa khoa Phương Đông
        </h1>
        <div class="flex flex-col lg:items-center justify-center md:justify-start w-full">
          <button
            @click="toggleSearch"
            class="cursor-pointer bg-button hover:bg-button text-white font-semibold py-2 lg:px-6 lg:py-3 px-4 rounded-full text-base flex max-w-36 items-center whitespace-nowrap justify-center "
          >
            <svg
              v-if="!showSearch"
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

            <svg
              v-else
              xmlns="http://www.w3.org/2000/svg"
              class="w-5 h-5"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
              stroke-width="2"
            >
              <!-- Icon đóng -->
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                d="M6 18L18 6M6 6l12 12"
              />
            </svg>

            {{ showSearch ? "Đóng tìm kiếm" : "Tìm bác sĩ" }}
          </button>

          <div v-if="showSearch" class="absolute max-w-32 w-1/3 lg:translate-y-1/1 translate-y-0 translate-x-10/8 lg:translate-x-0">
            <input
              v-model="searchQuery"
              type="text"
              placeholder="Tìm tên bác sĩ..."
              class="w-full lg:p-3 p-2 border rounded-3xl outline-none focus:ring focus:ring-green-300"
            />
          </div>
        </div>
      </div>

      <!-- bac si -->
      <!-- Bác sĩ chỉ số lẻ -->
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <div
          v-for="(doctor, index) in filteredDoctors.filter((_, i) => i % 2 !== 0)"
          :key="'odd-' + index"
          class="items-center rounded-lg justify-center lg:gap-8 gap-4 grid md:grid-cols-2 grid-cols-3"
        >
          <!-- image -->
          <div class="col-span-1 relative cursor-pointer">
            <div class="relative z-10 rounded-b-full lg:p-4 overflow-hidden">
              <img
                :src="doctor.image"
                :alt="doctor.name"
                class="object-contain translate-y-1/9"
              />
            </div>
            <div
              class="absolute rounded-full bg-gradient-mygreen w-full bottom-0 z-0 aspect-square"
            ></div>
          </div>
          <!-- profile -->
          <div
            class="md:col-span-1 col-span-2 flex justify-center flex-col translate-y-1/9 p-2"
          >
            <h2
              class="xl:text-lg lg:text-base md:text-sm text-2xs font-semibold whitespace-nowrap text-gray-900"
            >
              BS: {{ doctor.name }}
            </h2>
            <p class="text-gray-600 xl:text-base lg:text-sm md:text-xs text-[14px]">
              {{ doctor.title }}
            </p>
            <p class="text-gray-700 mt-2 xl:text-base lg:text-sm md:text-xs text-[14px]">
              Kinh nghiệm: <span class="font-bold">{{ doctor.experience }}</span>
            </p>
            <div class="flex items-center mt-1">
              <span class="text-gray-700 mr-2">Xếp hạng:</span>
              <div class="flex">
                <svg
                  v-for="n in doctor.rating"
                  :key="n"
                  class="w-5 h-5 text-yellow-400 fill-current"
                  viewBox="0 0 24 24"
                >
                  <path
                    d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2
            9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                  />
                </svg>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Bác sĩ chỉ số chẵn -->
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <div
          v-for="(doctor, index) in filteredDoctors.filter((_, i) => i % 2 === 0)"
          :key="'even-' + index"
          class="items-center rounded-lg justify-center lg:gap-8 gap-4 grid md:grid-cols-2 grid-cols-3"
        >
          <!-- profile -->
          <div
            class="md:col-span-1 col-span-2 flex justify-center flex-col translate-y-1/9 p-2"
          >
            <h2
              class="xl:text-lg lg:text-base md:text-sm text-2xs font-semibold whitespace-nowrap text-gray-900"
            >
              BS: {{ doctor.name }}
            </h2>
            <p class="text-gray-600 xl:text-base lg:text-sm md:text-xs text-[14px]">
              {{ doctor.title }}
            </p>
            <p class="text-gray-700 mt-2 xl:text-base lg:text-sm md:text-xs text-[14px]">
              Kinh nghiệm: <span class="font-bold">{{ doctor.experience }}</span>
            </p>
            <div class="flex items-center mt-1">
              <span class="text-gray-700 mr-2">Xếp hạng:</span>
              <div class="flex">
                <svg
                  v-for="n in doctor.rating"
                  :key="n"
                  class="w-5 h-5 text-yellow-400 fill-current"
                  viewBox="0 0 24 24"
                >
                  <path
                    d="M12 17.27L18.18 21l-1.64-7.03L22 9.24l-7.19-.61L12 2
            9.19 8.63 2 9.24l5.46 4.73L5.82 21z"
                  />
                </svg>
              </div>
            </div>
          </div>
          <!-- image -->
          <div class="col-span-1 relative cursor-pointer">
            <div class="relative z-10 rounded-b-full lg:p-4 overflow-hidden">
              <img
                :src="doctor.image"
                :alt="doctor.name"
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
  </div>
</template>

<script setup>
import { ref, computed } from "vue";
import NTCImage from "../Images/NTC.png";
import NHBImage from "../Images/NHB.png";
import TKTImage from "../Images/TKT.png";
import NTKYImage from "../Images/NTKY.png";

const showSearch = ref(false);
const searchQuery = ref("");

// Danh sách bác sĩ
const doctors = ref([
  {
    name: "NGUYỄN HUY BẠO",
    title: "PGS.TS. Bác sĩ Ung bướu - Phó giám đốc Bệnh viện Đa khoa Phương Đông",
    image: NHBImage,
    experience: "20 năm",
    rating: 5,
  },
  {
    name: "NGUYỄN TRUNG CHÍNH",
    title: "PGS.TS. Bác sĩ Ung bướu - Giám đốc Bệnh viện Đa khoa Phương Đông",
    image: NTCImage,
    experience: "20 năm",
    rating: 5,
  },

  {
    name: "NGUYỄN THỊ KIM YẾN",
    title: "PGS.TS. Bác sĩ Ung bướu - Phó giám đốc Bệnh viện Đa khoa Phương Đông",
    image: NTKYImage,
    experience: "20 năm",
    rating: 5,
  },
  {
    name: "TRẦN KINH TRANG",
    title: "PGS.TS. Bác sĩ Ung bướu - Phó giám đốc Bệnh viện Đa khoa Phương Đông",
    image: TKTImage,
    experience: "20 năm",
    rating: 5,
  },
]);

// Danh sách lọc theo tên
const filteredDoctors = computed(() => {
  if (!searchQuery.value.trim()) return doctors.value;
  return doctors.value.filter((doc) =>
    doc.name.toLowerCase().includes(searchQuery.value.trim().toLowerCase())
  );
});

const toggleSearch = () => {
  showSearch.value = !showSearch.value;
  searchQuery.value = "";
};
</script>

<style lang="scss" scoped></style>
