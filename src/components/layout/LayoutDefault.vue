<template>
  <div class="overflow-x-hidden h-screen w-screen">
    <Header />
    <Hero />

    <div class="relative w-full lg:mb-12">
      <div class="absolute top-0 w-7/20 -translate-y-1/2 left-1/6">
        <Ellipse />
      </div>
      <div class="relative mx-3 lg:top-12 top-6 w-full lg:left-2/15">
        <Banner />
      </div>
    </div>
    <!-- section 1 -->
    <div class="relative w-full lg:mb-12">
      <div class="absolute -bottom-1/2 w-3/10 -left-1/10">
        <Ellipse />
      </div>
      <div class="relative w-full">
        <Section1 />
      </div>
    </div>
    <!-- section 2 -->
    <div class="relative w-full lg:mb-12 top-2 mb-3">
      <div class="absolute -bottom-1/10 w-2/10 -right-1/20 z-10">
        <Ellipse />
      </div>
      <div class="relative w-full">
        <Section2 />
      </div>
    </div>

    <!-- section 3 -->
    <div class="relative w-full lg:mb-12 top-2">
      <div class="absolute translate-y-3/5 w-3/10 right-3/8 z-10">
        <Ellipse />
      </div>
      <div class="relative w-full">
        <Section3 />
      </div>
    </div>
  </div>
  <!-- section 4 -->
  <Section4/>
</template>

<script setup>
import Ellipse from "../Ellipse.vue";
import Header from "../Header.vue";
import Hero from "../Hero.vue";
import Banner from "../Banner.vue";
import Content from "../Content.vue";
import Section1 from "../Section1.vue";
import Section2 from "../Section2.vue";
import Section3 from "../Section3.vue";
import Section4 from "../section4.vue";
</script>

<style lang="scss" scoped></style>
