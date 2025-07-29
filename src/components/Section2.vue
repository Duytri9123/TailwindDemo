<template>
  <section>
    <div class="w-screen relative flex justify-center bg-gradient-greenblue">
      <div
        class="relative md:p-12 w-screen lg:w-9/10 rounded-b-3xl overflow-hidden drop-shadow-2xl/20 z-20"
      >
        <div class="bg-white rounded-b-3xl">
          <div class="lg:p-8 p-1">
            <div>
              <div>
                <!-- title -->
                <div class="flex lg:flex-row flex-col w-full p-4 bg-white text-center">
                  <div class="items-center gap-2">
                    <!-- Logo -->
                    <img
                      src="../Images/logo.png"
                      alt="Logo"
                      class="h-10 object-contain"
                    />
                  </div>
                  <div class="flex-1 text-center lg:pr-20">
                    <h1 class="font-medium 2xl:text-3xl xl:text-2xl lg:text-xl text-lg">
                      Bảng giá các dịch vụ khám và chữa bệnh:
                    </h1>
                    <p class="text-sm text-gray-500">
                      Ghi chú: Lorem ipsum dolor sit amet, consectetur adipiscing elit lis
                      iaculis ac felis
                    </p>
                  </div>
                </div>
              </div>
            </div>
            <div>
              <!-- table  -->
              <div>
                <div
                  class="bg-gradient-mygreen w-full overflow-hidden rounded-xl max-h-[550px] overflow-y-auto"
                >
                  <table
                    class="w-full table-auto text-sm bg-white border border-gray-200 rounded-3xl"
                  >
                    <thead>
                      <tr class="text-white">
                        <th
                          rowspan="2"
                          class="bg-teal-500 border border-gray-200 py-3 px-4 uppercase font-bold text-left w-[5%]"
                        >
                          STT
                        </th>
                        <th
                          rowspan="2"
                          class="bg-teal-500 border border-gray-200 py-3 px-4 uppercase font-bold text-left w-[45%]"
                        >
                          TÊN DỊCH VỤ
                        </th>
                        <th
                          colspan="2"
                          class="bg-teal-400 border border-gray-200 py-3 px-4 uppercase font-bold text-center w-[50%]"
                        >
                          GIÁ DỊCH VỤ DÀNH CHO KHÁCH HÀNG CÓ QUỐC TỊCH
                        </th>
                      </tr>
                      <tr class="text-white">
                        <th
                          class="bg-teal-400 border border-gray-200 py-2 px-4 font-normal text-center w-[25%]"
                        >
                          Việt Nam
                        </th>
                        <th
                          class="bg-teal-400 border border-gray-200 py-2 px-4 font-normal text-center w-[25%]"
                        >
                          Nước ngoài
                        </th>
                      </tr>
                    </thead>
                  </table>
                <div class="max-h-[450px] overflow-y-auto">
                  <table
                    class="w-full table-auto text-sm bg-white border border-t-0 border-gray-200"
                  >
                    <tbody class="text-gray-700">
                      <tr
                        class="bg-white hover:bg-emerald-100 transition-all duration-200"
                      >
                        <td class="py-3 px-4 text-center border border-gray-200">1</td>
                        <td class="py-3 px-4 border border-gray-200">
                          Chăm sóc điều dưỡng tại nhà - Bệnh nhân nặng
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          200,000/giờ
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          400,000/giờ
                        </td>
                      </tr>
                      <tr
                        class="bg-gray-50 hover:bg-emerald-100 transition-all duration-200"
                      >
                        <td class="py-3 px-4 text-center border border-gray-200">2</td>
                        <td class="py-3 px-4 border border-gray-200">Cắt chỉ</td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          300,000/lần
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          300,000/lần
                        </td>
                      </tr>
                      <tr
                        class="bg-white hover:bg-emerald-100 transition-all duration-200"
                      >
                        <td class="py-3 px-4 text-center border border-gray-200">3</td>
                        <td class="py-3 px-4 border border-gray-200">
                          Phương tiện bảo hộ lấy mẫu
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          300,000/lần
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          300,000/lần
                        </td>
                      </tr>
                      <tr
                        class="bg-gray-50 hover:bg-emerald-100 transition-all duration-200"
                      >
                        <td class="py-3 px-4 text-center border border-gray-200">4</td>
                        <td class="py-3 px-4 border border-gray-200">Tắm bé tại nhà</td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          300,000/lần
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          300,000/lần
                        </td>
                      </tr>
                      <tr
                        class="bg-white hover:bg-emerald-100 transition-all duration-200"
                      >
                        <td class="py-3 px-4 text-center border border-gray-200">5</td>
                        <td class="py-3 px-4 border border-gray-200">
                          Dẫn lưu nước tiểu bàng quang
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          300,000/lần
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          300,000/lần
                        </td>
                      </tr>
                      <tr
                        class="bg-gray-50 hover:bg-emerald-100 transition-all duration-200"
                      >
                        <td class="py-3 px-4 text-center border border-gray-200">6</td>
                        <td class="py-3 px-4 border border-gray-200">
                          Chăm sóc điều dưỡng tại nhà - Bệnh nhân nặng
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          200,000/giờ
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          400,000/giờ
                        </td>
                      </tr>
                      <tr
                        class="bg-white hover:bg-emerald-100 transition-all duration-200"
                      >
                        <td class="py-3 px-4 text-center border border-gray-200">7</td>
                        <td class="py-3 px-4 border border-gray-200">
                          Chăm sóc điều dưỡng tại nhà - Bệnh nhân nặng
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          200,000/giờ
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          400,000/giờ
                        </td>
                      </tr>
                      <tr
                        class="bg-gray-50 hover:bg-emerald-100 transition-all duration-200"
                      >
                        <td class="py-3 px-4 text-center border border-gray-200">8</td>
                        <td class="py-3 px-4 border border-gray-200">
                          Xét nghiệm tại nhà
                        </td>
                        <td
                          class="py-3 px-4 text-center border border-gray-200"
                          colspan="2"
                        >
                          Theo giá niêm yết tại BVĐK Phương Đông
                        </td>
                      </tr>
                      <tr
                        class="bg-white hover:bg-emerald-100 transition-all duration-200"
                      >
                        <td class="py-3 px-4 text-center border border-gray-200">9</td>
                        <td class="py-3 px-4 border border-gray-200">
                          Chăm sóc điều dưỡng tại nhà - Bệnh nhân nặng
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          200,000/giờ
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          400,000/giờ
                        </td>
                      </tr>
                      <tr
                        class="bg-gray-50 hover:bg-emerald-100 transition-all duration-200"
                      >
                        <td class="py-3 px-4 text-center border border-gray-200">10</td>
                        <td class="py-3 px-4 border border-gray-200">
                          Chăm sóc điều dưỡng tại nhà - Bệnh nhân nặng
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          200,000/giờ
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          400,000/giờ
                        </td>
                      </tr>
                      <tr
                        class="bg-white hover:bg-emerald-100 transition-all duration-200"
                      >
                        <td class="py-3 px-4 text-center border border-gray-200">11</td>
                        <td class="py-3 px-4 border border-gray-200">
                          Chăm sóc điều dưỡng tại nhà - Bệnh nhân nặng
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          200,000/giờ
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          400,000/giờ
                        </td>
                      </tr>
                    </tbody>
                  </table>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="w-full flex justify-center rounded-b-3xl bg-gradient-mygreen">
          <div class="flex whitespace-nowrap">
            <div>
              <a
                href="tel:19001806"
                class="hidden lg:flex flex-row items-center h-full rounded-[40px] px-4 pr-6 gap-2 text-white font-bold drop-shadow-md/25"
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
              class="w-fit px-4 py-2 rounded-md text-white flex items-center gap-2 font-bold drop-shadow-md/25"
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
