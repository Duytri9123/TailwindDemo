<template>
  <div class="overflow-hidden w-screen">
    <Header/>
    <Hero/>

    <!-- banner -->
    <div class="relative w-full ">
      <div class="absolute top-0 w-7/20 -translate-y-1/2 left-2/11">
        <Ellipse/>
      </div>
      <div class="relative transform lg:translate-y-1/6 mx-2 w-full">
        <Banner/>
      </div>
    </div>
    <!-- section 1 -->
    <div class="relative w-full">
      <div class="absolute -bottom-2/3 w-4/10 -left-1/8">
        <Ellipse/>
      </div>
      <div class="relative w-full transform lg:translate-y-1/20">
        <Section1/>
      </div>
    </div>
    <!-- section 2 -->
    <div class="relative w-full lg:top-2 mb-3">
      <div class="absolute -bottom-3/10 w-3/10 -right-1/15 z-10">
        <Ellipse/>
      </div>
      <div class="relative w-full">
        <Section2/>
      </div>
    </div>

    <!-- section 3 -->
    <div class="relative w-full">
      <div class="absolute translate-y-9/20 w-3/10 right-1/3 z-10">
        <Ellipse/>
      </div>
      <div class="relative w-full">
        <Section3/>
      </div>
    </div>
    <!-- section 4 -->
    <Section4 />
    <!-- section 5 -->
    <div class="relative w-full top-2">
      <div class="absolute w-3/10 -left-1/10 top-0">
        <Ellipse/>
      </div>
      <div class="relative  w-full">
        <Section5/>
      </div>
    </div>
    <!-- section 6 -->
    <div class="relative w-full lg:mb-28 mb-8 top-2">
      <div class="absolute w-3/10 -right-1/10 -translate-y-1/2 z-0">
        <Ellipse/>
      </div>
      <div class="relative w-full flex justify-center">
        <Section6/>
      </div>
      <div class="absolute w-2/10 bottom-0 -left-1/12">
        <Ellipse/>
      </div>
    </div>
    <!-- section 7 -->
    <div class="relative w-full lg:mb-28 mb-5 flex justify-center">
      <div class="absolute w-4/10 top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2">
        <Ellipse/>
      </div>
      <div class="relative w-full flex justify-center">
        <Section7/>
      </div>
    </div>

    <div class="relative w-full lg:mb-12 flex justify-center">
      <div class="relative w-full flex justify-center">
        <Section8/>
      </div>
    </div>

    <div class="relative w-full lg:mb-12 flex justify-center">
      <div class="relative w-full flex justify-center">
        <Section9/>
      </div>
    </div>
    <Footer/>
  </div>
</template>

<script setup>
import Ellipse from "../Ellipse.vue";
import Header from "../Header.vue";
import Hero from "../Hero.vue";
import Banner from "../Banner.vue";
import Section1 from "../Section1.vue";
import Section2 from "../Section2.vue";
import Section3 from "../Section3.vue";
import Section4 from "../Section4.vue";
import Section5 from "../Section5.vue";
import Section6 from "../Section6.vue";
import Section7 from "../Section7.vue";
import Section8 from "../Section8.vue";
import Section9 from "../Section9.vue";
import Footer from "../Footer.vue";
</script>

<style lang="scss" scoped></style>
