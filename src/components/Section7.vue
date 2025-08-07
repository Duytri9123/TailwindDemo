<template>
  <div class="flex justify-center items-center">
    <section class="w-8/9 xl:w-6/8 grid lg:grid-cols-2 grid-cols-1 lg:gap-8 gap-4">
      <div
        class="relative w-full overflow-hidden rounded-t-2xl rounded-br-2xl md:rounded-t-3xl md:rounded-br-3xl lg:rounded-t-4xl lg:rounded-br-4xl"
      >
        <img
          v-if="!isPlaying"
          @click="openVideo"
          src="../Images/male-female-doctor.jpg"
          alt="premature-baby"
          class="w-full 2xl:aspect-video lg:aspect-square object-cover"
        />
        <div
          v-if="!isPlaying"
          class="absolute top-1/2 -translate-y-1/2 left-1/2 -translate-x-1/2 cursor-pointer"
          @click="openVideo"
        >
          <svg
            width="73"
            height="52"
            viewBox="0 0 73 52"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <g clip-path="url(#clip0_1_13694)">
              <path
                d="M71.3875 8.00095C70.9688 6.4545 70.1521 5.04465 69.0186 3.91178C67.8851 2.77892 66.4744 1.96258 64.927 1.54405C59.2621 0 36.4627 0 36.4627 0C36.4627 0 13.6622 0.0467374 7.9973 1.59079C6.4499 2.00934 5.03922 2.82573 3.90572 3.95864C2.77223 5.09156 1.95548 6.50147 1.5368 8.04798C-0.176701 18.1074 -0.8414 33.4356 1.58385 43.0926C2.00257 44.639 2.81934 46.0489 3.95283 47.1818C5.08632 48.3146 6.49699 49.131 8.04435 49.5495C13.7093 51.0935 36.5092 51.0935 36.5092 51.0935C36.5092 51.0935 59.3089 51.0935 64.9735 49.5495C66.5209 49.131 67.9317 48.3147 69.0652 47.1818C70.1988 46.049 71.0156 44.6391 71.4343 43.0926C73.2416 33.0189 73.7985 17.7004 71.3875 8.00124V8.00095Z"
                fill="#FF0000"
              />
              <path
                d="M29.2059 36.4952L48.1198 25.5466L29.2059 14.5981V36.4952Z"
                fill="white"
              />
            </g>
            <defs>
              <clipPath id="clip0_1_13694">
                <rect width="73" height="51.2973" fill="white" />
              </clipPath>
            </defs>
          </svg>
        </div>

        <div
          v-if="isPlaying"
          @click.self="isPlaying = false"
          class="fixed inset-0 bg-black/40 bg-opacity-80 z-50 flex items-center justify-center"
        >
          <div class="relative w-full max-w-7xl aspect-video px-4">
            <iframe
              :src="youtubeUrl"
              class="w-full h-full rounded-xl shadow-lg"
              frameborder="0"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
              allowfullscreen
            ></iframe>
            <!-- Nút đóng -->
            <button
              class="absolute -top-4 -right-4 bg-white text-black rounded-full p-2 shadow-md hover:bg-red-500 hover:text-white transition"
              @click="isPlaying = false"
            >
              <svg
                xmlns="http://www.w3.org/2000/svg"
                class="w-6 h-6"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
                stroke-width="2"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  d="M6 18L18 6M6 6l12 12"
                />
              </svg>
            </button>
          </div>
        </div>
      </div>

      <div class="w-full p-1 flex flex-col lg:gap-10 gap-6">
        <div class="flex flex-col lg:gap-10 gap-6">
          <h1 class="text-lg md:text-2xl lg:text-2xl xl:text-4xl font-medium">
            Giải pháp an toàn hãy lựa chọn dịch vụ thai sản trọn gói tại bệnh viện Phương
            Đông
          </h1>
          <p class="text-gray-600 tracking-[0.5px] text-sm md:text-base">
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris ut risus
            luctus donec Lorem malesuada scelerisque euismod ullamcorper ac lacus aliquet
            quisque. Pulvinar aenean fusce pulvinar elementum odio dolor lorem aenean
            quis. Ridiculus mattis.
          </p>
        </div>
        <div
          class="max-w-60 flex items-center lg;text-base text-sm justify-start whitespace-nowrap"
        >
          <a
            href="tel:19001806"
            class="cursor-pointer flex flex-row items-center h-full rounded-4xl lg:px-6 lg:py-3 py-2 px-4 gap-2 text-white font-medium bg-button hover:bg-button drop-shadow-md/25"
          >
            <svg
              width="24"
              height="25"
              viewBox="0 0 24 25"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M18.965 17.4973L17.792 16.3243C17.206 15.7383 16.256 15.7383 15.671 16.3243L14.749 17.2463C14.543 17.4523 14.231 17.5213 13.965 17.4043C12.629 16.8193 11.309 15.9323 10.132 14.7553C8.96002 13.5833 8.07602 12.2693 7.49002 10.9383C7.36802 10.6633 7.43902 10.3403 7.65202 10.1273L8.47802 9.3013C9.14902 8.6303 9.14902 7.6813 8.56302 7.0953L7.39002 5.9223C6.60902 5.1413 5.34302 5.1413 4.56202 5.9223L3.91002 6.5733C3.16902 7.3143 2.86002 8.3833 3.06002 9.4433C3.55402 12.0563 5.07202 14.9173 7.52102 17.3663C9.97003 19.8153 12.831 21.3333 15.444 21.8273C16.504 22.0273 17.573 21.7183 18.314 20.9773L18.965 20.3263C19.746 19.5453 19.746 18.2793 18.965 17.4973Z"
                fill="white"
                stroke="white"
                stroke-width="0.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M13 7.8783C14.031 7.8643 15.067 8.2463 15.854 9.0333"
                stroke="white"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M18.682 6.20529C17.113 4.63629 15.056 3.85129 13 3.85129"
                stroke="white"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M17.009 11.8873C17.023 10.8563 16.641 9.82029 15.854 9.03329"
                stroke="white"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M18.682 6.20529C20.251 7.77429 21.036 9.83129 21.036 11.8873"
                stroke="white"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>

            <span>Liên hệ ngay</span>
          </a>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
import { ref } from "vue";

const isPlaying = ref(false);
const youtubeUrl = ref("");
const originalUrl =
  "https://www.youtube.com/watch?v=PU3kx8Qv43Y";

function openVideo() {
  isPlaying.value = true;
  youtubeUrl.value = convertYoutubeLinkToEmbed(originalUrl, true); // Tự động play
}

function closeVideo() {
  isPlaying.value = false;
  youtubeUrl.value = "";
}

function convertYoutubeLinkToEmbed(url, autoplay = false) {
  try {
    const youtube = new URL(url);

    // Nếu là playlist
    if (youtube.pathname === "/watch" && youtube.searchParams.get("list")) {
      const listId = youtube.searchParams.get("list");
      return `https://www.youtube.com/embed/videoseries?list=${listId}${
        autoplay ? "&autoplay=1" : ""
      }`;
    }

    // Nếu là video đơn
    const videoId = youtube.searchParams.get("v");
    if (videoId) {
      return `https://www.youtube.com/embed/${videoId}${autoplay ? "?autoplay=1" : ""}`;
    }

    return url;
  } catch (error) {
    return url;
  }
}
</script>

<style scoped></style>
