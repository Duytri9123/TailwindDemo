<template>
  <section>
    <div
      class="w-screen relative flex justify-center bg-gradient-greenblue lg:mt-28 md:px-10 px-1"
    >
      <div
        class="relative z-50 lg:pt-20 pt-10 w-screen lg:w-8/10 rounded-b-3xl drop-shadow-2xl/20 border-gradient xl:mb-20 lg:mb-12 mb-6 flex items-center justify-center"
      >
        <div class="bg-white rounded-b-3xl overflow-x-auto">
          <div class="lg:p-6 p-2">
            <div>
              <div>
                <!-- title -->
                <div
                  class="flex lg:flex-row flex-col w-full p-4 bg-white text-center items-center gap-2"
                >
                  <div class="items-center gap-2">
                    <!-- Logo -->
                    <img
                      src="../Images/logo.png"
                      alt="Logo"
                      class="h-10 object-contain"
                    />
                  </div>
                  <div class="flex-1 text-center lg:pr-20">
                    <h1 class="font-medium 2xl:text-4xl xl:text-3xl lg:text-2xl text-xl">
                      Bảng giá các dịch vụ khám và chữa bệnh:
                    </h1>
                    <p class="lg:text-base text-sm text-gray-500">
                      Ghi chú: Lorem ipsum dolor sit amet, consectetur adipiscing elit lis
                      iaculis ac felis
                    </p>
                  </div>
                </div>
              </div>
            </div>

            <!-- table  -->
            <div
              class="bg-gradient-mygreen w-full rounded-xl max-h-[550px] overflow-hidden"
            >
              <table
                class="w-full table-fixed lg:text-base tracking-[0.1px] md:text-sm text-xs border border-gray-200 rounded-t-xl"
              >
                <thead class="bg-gradient-mygreen text-white sticky top-0 z-10">
                  <tr>
                    <th
                      rowspan="2"
                      class="border border-gray-200 py-3 uppercase font-medium text-center lg:lg:w-[5%] w-[10%]"
                    >
                      STT
                    </th>
                    <th
                      rowspan="2"
                      class="border border-gray-200 py-3 px-4 uppercase font-medium text-center lg:w-[45%] w-[40%]"
                    >
                      TÊN DỊCH VỤ
                    </th>
                    <th
                      colspan="2"
                      class="border border-gray-200 py-3 px-4 uppercase font-medium text-center w-[49%]"
                    >
                      GIÁ DỊCH VỤ DÀNH CHO KHÁCH HÀNG CÓ QUỐC TỊCH
                    </th>
                    <th
                      rowspan="2"
                      class="border border-gray-200 py-3 uppercase font-medium text-center lg:w-4 md:w-1"
                    ></th>
                  </tr>
                  <tr>
                    <th
                      class="border border-gray-200 py-2 px-4 font-medium text-center w-[25%]"
                    >
                      Việt Nam
                    </th>
                    <th
                      class="border border-gray-200 py-2 px-4 font-medium text-center w-[25%]"
                    >
                      Nước ngoài
                    </th>
                  </tr>
                </thead>
              </table>

              <div class="max-h-[400px]  overflow-y-auto w-full">
                <table
                  class="w-full table-fixed lg:text-base md:text-sm text-xs border border-gray-200"
                >
                  <tbody>
                    <tr class="bg-white hover:bg-emerald-100 transition-all duration-200">
                      <td
                        class="lg:w-[5%] w-[10%] py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        1
                      </td>
                      <td
                        class="lg:w-[45%] w-[40%] px-4 py-3 border border-gray-200 text-gray-700"
                      >
                        Chăm sóc điều dưỡng tại nhà - Bệnh nhân nặng
                      </td>
                      <td
                        class="w-[25%] px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        200,000/giờ
                      </td>
                      <td
                        class="w-[25%] px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        400,000/giờ
                      </td>
                    </tr>

                    <tr
                      class="bg-gray-50 hover:bg-emerald-100 transition-all duration-200"
                    >
                      <td class="py-3 border border-gray-200 text-gray-700 text-center">
                        2
                      </td>
                      <td class="px-4 py-3 border border-gray-200 text-gray-700">
                        Cắt chỉ
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        300,000/lần
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        300,000/lần
                      </td>
                    </tr>

                    <tr class="bg-white hover:bg-emerald-100 transition-all duration-200">
                      <td class="py-3 border border-gray-200 text-gray-700 text-center">
                        3
                      </td>
                      <td class="px-4 py-3 border border-gray-200 text-gray-700">
                        Phương tiện bảo hộ lấy mẫu
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        300,000/lần
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        300,000/lần
                      </td>
                    </tr>

                    <tr
                      class="bg-gray-50 hover:bg-emerald-100 transition-all duration-200"
                    >
                      <td class="py-3 border border-gray-200 text-gray-700 text-center">
                        4
                      </td>
                      <td class="px-4 py-3 border border-gray-200 text-gray-700">
                        Tắm bé tại nhà
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        300,000/lần
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        300,000/lần
                      </td>
                    </tr>

                    <tr class="bg-white hover:bg-emerald-100 transition-all duration-200">
                      <td class="py-3 border border-gray-200 text-gray-700 text-center">
                        5
                      </td>
                      <td class="px-4 py-3 border border-gray-200 text-gray-700">
                        Dẫn lưu nước tiểu bàng quang
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        300,000/lần
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        300,000/lần
                      </td>
                    </tr>

                    <tr
                      class="bg-gray-50 hover:bg-emerald-100 transition-all duration-200"
                    >
                      <td class="py-3 border border-gray-200 text-gray-700 text-center">
                        6
                      </td>
                      <td class="px-4 py-3 border border-gray-200 text-gray-700">
                        Chăm sóc điều dưỡng tại nhà - Bệnh nhân nặng
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        200,000/giờ
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        400,000/giờ
                      </td>
                    </tr>

                    <tr class="bg-white hover:bg-emerald-100 transition-all duration-200">
                      <td class="py-3 border border-gray-200 text-gray-700 text-center">
                        7
                      </td>
                      <td class="px-4 py-3 border border-gray-200 text-gray-700">
                        Chăm sóc điều dưỡng tại nhà - Bệnh nhân nặng
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        200,000/giờ
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        400,000/giờ
                      </td>
                    </tr>

                    <tr
                      class="bg-gray-50 hover:bg-emerald-100 transition-all duration-200"
                    >
                      <td class="py-3 border border-gray-200 text-gray-700 text-center">
                        8
                      </td>
                      <td class="px-4 py-3 border border-gray-200 text-gray-700">
                        Xét nghiệm tại nhà
                      </td>
                      <td
                        colspan="2"
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        Theo giá niêm yết tại BVĐK Phương Đông
                      </td>
                    </tr>

                    <tr class="bg-white hover:bg-emerald-100 transition-all duration-200">
                      <td class="py-3 border border-gray-200 text-gray-700 text-center">
                        9
                      </td>
                      <td class="px-4 py-3 border border-gray-200 text-gray-700">
                        Chăm sóc điều dưỡng tại nhà - Bệnh nhân nặng
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        200,000/giờ
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        400,000/giờ
                      </td>
                    </tr>

                    <tr
                      class="bg-gray-50 hover:bg-emerald-100 transition-all duration-200"
                    >
                      <td class="py-3 border border-gray-200 text-gray-700 text-center">
                        10
                      </td>
                      <td class="px-4 py-3 border border-gray-200 text-gray-700">
                        Chăm sóc điều dưỡng tại nhà - Bệnh nhân nặng
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        200,000/giờ
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        400,000/giờ
                      </td>
                    </tr>
                    <tr
                      class="bg-gray-50 hover:bg-emerald-100 transition-all duration-200"
                    >
                      <td class="py-3 border border-gray-200 text-gray-700 text-center">
                        11
                      </td>
                      <td class="px-4 py-3 border border-gray-200 text-gray-700">
                        Chăm sóc điều dưỡng tại nhà - Bệnh nhân nặng
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        200,000/giờ
                      </td>
                      <td
                        class="px-4 py-3 border border-gray-200 text-gray-700 text-center"
                      >
                        400,000/giờ
                      </td>
                    </tr>
                  </tbody>
                </table>
              </div>
            </div>
          </div>
          <div class="w-full flex justify-center rounded-b-3xl bg-gradient-mygreen">
            <div class="flex lg:flex-row flex-col items-center justify-center my-1">
              <div>
                <a  
                  href="tel:19001806"
                  class="flex flex-row items-center h-full rounded-[40px] px-4 md:pr-6 gap-2 text-white whitespace-nowrap text-xs md:text-sm lg:text-base"
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
                      d="M18.965 16.6102L17.792 15.4372C17.206 14.8512 16.256 14.8512 15.671 15.4372L14.749 16.3592C14.543 16.5652 14.231 16.6342 13.965 16.5172C12.629 15.9322 11.309 15.0452 10.132 13.8682C8.96002 12.6962 8.07602 11.3822 7.49002 10.0512C7.36802 9.77621 7.43902 9.45321 7.65202 9.24021L8.47802 8.41421C9.14902 7.74321 9.14902 6.79421 8.56302 6.20821L7.39002 5.03521C6.60902 4.25421 5.34302 4.25421 4.56202 5.03521L3.91002 5.68621C3.16902 6.42721 2.86002 7.49621 3.06002 8.55621C3.55402 11.1692 5.07202 14.0302 7.52102 16.4792C9.97002 18.9282 12.831 20.4462 15.444 20.9402C16.504 21.1402 17.573 20.8312 18.314 20.0902L18.965 19.4392C19.746 18.6582 19.746 17.3922 18.965 16.6102V16.6102Z"
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
                      d="M18.682 5.31811C17.113 3.74911 15.056 2.96411 13 2.96411"
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
                      d="M18.682 5.31812C20.251 6.88712 21.036 8.94412 21.036 11.0001"
                      stroke="white"
                      stroke-width="1.5"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>

                  <span>Hotline: 1900 1806</span>
                </a>
              </div>

              <div
                class="w-fit px-4 py-2 rounded-md text-white flex items-center gap-2 md:text-sm lg:text-base text-xs"
              >
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M12 3.1001C16.667 8.0271 16.667 15.9731 12 20.9001"
                    stroke="white"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M12 20.9001C7.33301 15.9731 7.33301 8.0271 12 3.1001"
                    stroke="white"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M12 3C16.982 3 21 7.018 21 12C21 16.982 16.982 21 12 21"
                    stroke="white"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M12 21C7.018 21 3 16.982 3 12C3 7.018 7.018 3 12 3"
                    stroke="white"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M3.51001 9H20.49"
                    stroke="white"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M3.51001 15H20.49"
                    stroke="white"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>

                <a
                  href="https://benhvienphuongdong.vn/"
                  target="_blank"
                  class="hover:underline"
                >
                  https://benhvienphuongdong.vn/
                </a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup></script>

<style lang="scss" scoped></style>
