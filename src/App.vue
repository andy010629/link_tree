<script setup lang="ts">
import LinkButton from './components/LinkButton.vue'


const link_data = [
   { title:'個人網站', url:'https://nulong.me'},
  { title:'好保 - 投資型保單整合平台', url:'https://haobao.nulong.me'},
  { title:'好保介紹投影片', url:'https://haobao.nulong.me'},
  { title:'布林科技', url:'https://bullinv.tech'},
  { title:'外匯策略管理後台', url:'https://fx.bullinv.tech'},
  { title:'台主記錄器', url:'https://claw.nulong.me'},
  { title:'演算法實作', url:'https://algohw.nulong.me'},
  // { title:'國家與市場 - 主持人投影片', url:'https://docs.google.com/presentation/d/103EdDxqWLoLa2F6ocIBfpbboU1zC9fEnAT3-yeF-Mwc/edit?usp=sharing'}
]

</script>

<template>
  <div>
    <div class="w-full flex justify-center text-4xl font-bold text-gray-200 tracking-wider">個人連結 mylink</div>
    <div class="w-full mt-12 grid  grid-cols-1 md:grid-cols-3 gap-6 md:gap-12">
      <LinkButton v-for="link in link_data" :key="link.title" :title="link.title" :url="link.url" />
    </div>
    <div class="h-24"></div>
  </div>
</template>

<style scoped>

</style>
