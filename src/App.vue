<script setup>

import Header from '@/components/Header.vue';
import Banner from './components/Banner.vue';
import Footer from '@/components/Footer.vue';

</script>

<template>

  <template></template>

  <Header />

  <main>
      
    <Banner>
      15% off!
      <template v-slot:text>Buy now while stocks last!</template>
      <template v-slot:['banner-btn']>Buy right now!</template>
    </Banner>

    <Banner>
      SALE
      <template v-slot:['banner-btn']>this is the button text</template>
    </Banner>

  </main>

  <Footer />

</template>

<style>

*{
  margin: 0;
  padding: 0;
}

main{
  height: 100vh;
}

</style>
