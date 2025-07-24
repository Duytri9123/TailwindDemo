<template>
  <section>
    <div
      class="w-screen relative flex justify-center"
      style="background: var(--my-gradient)"
    >
      <div class="relative md:p-12 w-screen lg:w-8/10 rounded-b-3xl overflow-hidden drop-shadow-2xl/20">
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
            <div >
              <!-- table  -->
              <div>
                <div
                  class="bg-gradient-to-r from-[var(--color-green)] to-[var(--color-blue)] w-full overflow-hidden rounded-xl"
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

                    <tbody class="text-gray-700">
                      <tr class="bg-white">
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
                      <tr class="bg-gray-50">
                        <td class="py-3 px-4 text-center border border-gray-200">2</td>
                        <td class="py-3 px-4 border border-gray-200">Cắt chỉ</td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          300,000/lần
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          300,000/lần
                        </td>
                      </tr>
                      <tr class="bg-white">
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
                      <tr class="bg-gray-50">
                        <td class="py-3 px-4 text-center border border-gray-200">4</td>
                        <td class="py-3 px-4 border border-gray-200">Tắm bé tại nhà</td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          300,000/lần
                        </td>
                        <td class="py-3 px-4 text-center border border-gray-200">
                          300,000/lần
                        </td>
                      </tr>
                      <tr class="bg-white">
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
                      <tr class="bg-gray-50">
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
                      <tr class="bg-white">
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
                      <tr class="bg-gray-50">
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
                      <tr class="bg-white">
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
                      <tr class="bg-gray-50">
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
                      <tr class="bg-white">
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

          <div
            class="w-full flex justify-center rounded-b-3xl bg-gradient-to-r from-[var(--color-green)] to-[var(--color-blue)]"
          >
            <div class="flex whitespace-nowrap">
              <div>
                <a
                  href="tel:19001806"
                  class="hidden lg:flex flex-row items-center h-full rounded-[40px] px-4 pr-6 gap-2 text-white font-bold drop-shadow-md/25"
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
              </div>

              <div
                class="w-fit px-4 py-2 rounded-md text-white flex items-center gap-2 font-bold drop-shadow-md/25"
              >
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  class="w-5 h-5"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    stroke-width="2"
                    d="M12 2a10 10 0 100 20 10 10 0 000-20zm0 0c2.21 0 4 4.03 4 9s-1.79 9-4 9-4-4.03-4-9 1.79-9 4-9zm0 0v18"
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
