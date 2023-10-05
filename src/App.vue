<script setup>
import { RouterLink, RouterView, useRoute  } from 'vue-router'
import  Header from '@/components/Header.vue'
import  Footer from '@/components/Footer.vue'
</script>


<template >
  <Header />
  <RouterView />
  <!-- <Footer /> -->
</template>


<style>
    body{
        background: #222;
    }

    
</style>