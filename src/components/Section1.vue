<template>
  <section
    class="w-screen flex lg:flex-row flex-col lg:gap-10 gap-4 items-center justify-between px-6 mb-10"
  >
    <!-- img -->
    <div class="w-full lg:w-1/2 flex justify-center lg:justify-end">
      <div
        class="md:w-3/4 w-full overflow-hidden xl:aspect-[10/9] lg:aspect-[3/5] lg:rounded-b-[var(--g-80)] lg:rounded-tr-[var(--g-80)] rounded-b-[var(--g-40)] rounded-tr-[var(--g-40)]"
      >
        <img src="../Images/h1.jpg" alt="" class="w-full h-full object-cover shadow-lg" />
      </div>
    </div>
    <!-- dich vu -->
    <div class="w-full lg:w-1/2 space-y-4 flex justify-center flex-col gap-2">
      <div class="flex flex-col lg:gap-4 gap-2">
        <span class="text-nowrap font-semibold lg:text-4xl md:text-xl text-lg align-top"
          >Dịch vụ thai sản trọn gói</span
        >
        <span class="text-sm md:text-base text-gray-500 tracking-[0.5px] lg:w-3/4">
          Mang thai và sinh nở là một hành trình vô cùng kỳ diệu nhưng cũng lắm mệt mỏi,
          áp lực, thậm chí là nguy hiểm. Thấu hiểu nỗi niềm đó, dịch vụ thai sản trọn gói
          Phương Đông nhằm mang tới trải nghiệm nhẹ nhàng, an tâm cho người mẹ trong suốt
          thai kỳ, ngày vượt cạn đến sau sinh và sự chăm sóc toàn diện với em bé ngay từ
          giây phút đầu tiên chào đời.</span
        >
      </div>
      <!-- ul -->
      <ul class="list-none pl-0 space-y-4 text-black font-medium gap-2">
        <li class="flex items-start gap-2 ml-0 even:ml-4">
          <span class="w-3 h-3 rounded-full bg-gradient-mygreen mt-1 shrink-0"></span>
          <span class="text-sm md:text-base tracking-[0.1px]"
            >Đội ngũ bác sĩ sản khoa giàu kinh nghiệm</span
          >
        </li>
        <li class="flex items-start gap-2 ml-0 even:ml-4">
          <span class="w-3 h-3 rounded-full bg-gradient-mygreen mt-1 shrink-0"></span>
          <span class="text-sm md:text-base tracking-[0.1px]"
            >Chăm sóc mẹ và bé toàn diện trước trong và sau sinh</span
          >
        </li>
        <li class="flex items-start gap-2 ml-0 even:ml-4">
          <span class="w-3 h-3 rounded-full bg-gradient-mygreen mt-1 shrink-0"></span>
          <span class="text-sm md:text-base tracking-[0.1px]"
            >Không gian đẳng cấp với trang thiết bị y tế hiện đại</span
          >
        </li>
        <li class="flex items-start gap-2 ml-0 even:ml-4">
          <span class="w-3 h-3 rounded-full bg-gradient-mygreen mt-1 shrink-0"></span>
          <span class="text-sm md:text-base tracking-[0.1px]"
            >Đi sinh sung sướng như đi nghỉ dưỡng</span
          >
        </li>
        <li class="flex items-start gap-2 ml-0 even:ml-4">
          <span class="w-3 h-3 rounded-full bg-gradient-mygreen mt-1 shrink-0"></span>
          <span class="text-sm md:text-base tracking-[0.1px]"
            >Con yêu chào đời với những điều kiện tốt nhất</span
          >
        </li>
        <li class="flex items-start gap-2 ml-0 even:ml-4">
          <span class="w-3 h-3 rounded-full bg-gradient-mygreen mt-1 shrink-0"></span>
          <span class="text-sm md:text-base tracking-[0.1px]"
            >Thanh toán đồng thời bảo hiểm Y tế, bảo hiểm bảo lãnh</span
          >
        </li>
        <li class="flex items-start gap-2 ml-0 even:ml-4">
          <span class="w-3 h-3 rounded-full bg-gradient-mygreen mt-1 shrink-0"></span>
          <span class="text-sm md:text-base tracking-[0.1px]"
            >Bảng giá các gói sinh tại Bệnh viện Phương Đông</span
          >
        </li>
      </ul>

      <a
        href="tel:123456"
        class="cursor-pointer relative left-0 max-w-30 mt-2 px-5 py-2 md:px-6 md:py-3 bg-button hover:bg-button drop-shadow-2xl/20 rounded-full text-white text-xs sm:text-sm lg:text-base font-semibold text-nowrap text-center"
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
            d="M18.965 16.61L17.792 15.437C17.206 14.851 16.256 14.851 15.671 15.437L14.749 16.359C14.543 16.565 14.231 16.634 13.965 16.517C12.629 15.932 11.309 15.045 10.132 13.868C8.96002 12.696 8.07602 11.382 7.49002 10.051C7.36802 9.77597 7.43902 9.45297 7.65202 9.23997L8.47802 8.41397C9.14902 7.74297 9.14902 6.79397 8.56302 6.20797L7.39002 5.03497C6.60902 4.25397 5.34302 4.25397 4.56202 5.03497L3.91002 5.68597C3.16902 6.42697 2.86002 7.49597 3.06002 8.55597C3.55402 11.169 5.07202 14.03 7.52102 16.479C9.97003 18.928 12.831 20.446 15.444 20.94C16.504 21.14 17.573 20.831 18.314 20.09L18.965 19.439C19.746 18.658 19.746 17.392 18.965 16.61Z"
            fill="white"
            stroke="white"
            stroke-width="1.5"
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
            d="M18.6821 5.31787C20.2511 6.88687 21.0361 8.94387 21.0361 10.9999"
            stroke="white"
            stroke-width="1.5"
            stroke-linecap="round"
            stroke-linejoin="round"
          />
        </svg>

        GỌI CHO CHÚNG TÔI
      </a>
    </div>
  </section>
</template>

<script setup></script>

<style lang="scss" scoped></style>
