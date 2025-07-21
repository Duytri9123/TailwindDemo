<template>
  <div>
    <Header />
    <Hero />
    <div class="absolute top-[378px] left-[340px] w-[600px] h-[600px] z-0">
      <Ellipse />
    </div>
  </div>
</template>

<script setup>
import Ellipse from "../Ellipse.vue";
import Header from "../Header.vue";
import Hero from "../Hero.vue";
</script>

<style lang="scss" scoped></style>
