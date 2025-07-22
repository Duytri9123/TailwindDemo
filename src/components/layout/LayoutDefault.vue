<template>
  <div>
    <Header />
    <Hero />

    <div class="relative w-full">
      <div class="relative top-0 w-7/20 -translate-y-1/2 left-2/12">
        <Ellipse />
      </div>
      <div class="absolute top-1/7 w-full left-2/15">
        <SideBar />
      </div>
    </div>
  </div>
</template>

<script setup>
import Ellipse from "../Ellipse.vue";
import Header from "../Header.vue";
import Hero from "../Hero.vue";
import SideBar from "../SideBar.vue";
</script>

<style lang="scss" scoped></style>
