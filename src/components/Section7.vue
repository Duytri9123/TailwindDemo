<template>
  <section class="w-7/8 grid lg:grid-cols-2 grid-cols-1">
    <div
      class="relative w-full overflow-hidden rounded-t-2xl rounded-br-2xl md:rounded-t-3xl md:rounded-br-3xl lg:rounded-t-4xl lg:rounded-br-4xl"
    >
      <img
        v-if="!isPlaying"
        src="../Images/male-female-doctor.jpg"
        alt="premature-baby"
        class="w-full h-full object-cover"
      />
      <div
        v-if="!isPlaying"
        class="absolute top-1/2 -translate-y-1/2 left-1/2 -translate-x-1/2 cursor-pointer"
        @click="isPlaying = true"
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

      <iframe
        v-if="isPlaying"
        class="absolute top-0 left-0 w-full h-full min-h-60"
        :src="youtubeUrl"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
      ></iframe>
    </div>

    <div class="w-full md:p-8 p-1 space-y-10">
      <div>
        <h1 class="text-lg md:text-xl lg:text-2xl xl:text-3xl font-bold mb-4">
          Giải pháp an toàn hãy lựa chọn dịch vụ thai sản trọn gói tại bệnh viện Phương Đông
        </h1>
        <p class="text-gray-600">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris ut risus luctus
          donec Lorem malesuada scelerisque euismod ullamcorper ac lacus aliquet quisque.
          Pulvinar aenean fusce pulvinar elementum odio dolor lorem aenean quis. Ridiculus
          mattis.
        </p>
      </div>
      <div class="max-w-40 h-10">
        <a
          href="tel:19001806"
          class="hidden lg:flex flex-row items-center h-full rounded-4xl px-4 pr-6 gap-2 text-white font-bold bg-button hover:bg-button drop-shadow-md/25"
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
          <span>Liên hệ ngay</span>
        </a>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref } from 'vue'

const isPlaying = ref(false)

const youtubeUrl = ref(convertYoutubeLinkToEmbed(originalUrl))

const originalUrl = 'https://www.youtube.com/watch?v=2Z-N3AxPJwM&list=RD2Z-N3AxPJwM&start_radio=1'

function convertYoutubeLinkToEmbed(url) {
  try {
    const youtube = new URL(url)

    if (youtube.pathname === '/watch' && youtube.searchParams.get('list')) {
      const listId = youtube.searchParams.get('list')
      return `https://www.youtube.com/embed/videoseries?list=${listId}`
    }

    const videoId = youtube.searchParams.get('v')
    if (videoId) {
      return `https://www.youtube.com/embed/${videoId}`
    }

    return url
  } catch (error) {
    return url
  }
}
</script>

<style scoped></style>
