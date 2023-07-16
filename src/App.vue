<script setup lang="ts">
import LinkButton from './components/LinkButton.vue'


const link_data = [
   { title:'個人網站', url:'https://nulong.me'},
  { title:'好保 - 投資型保單整合平台', url:'https://haobao.nulong.me'},
  { title:'好保介紹投影片', url:'https://docs.google.com/presentation/d/1PrH4r_pKdyZetbc1M7oalVx56dkJ1Lcy7hgKbxgq6yA/edit?usp=sharing'},
  { title:'布林科技', url:'https://bullinv.tech'},
  { title:'外匯策略管理後台', url:'https://fx.bullinv.tech'},
  // { title:'台主記錄器', url:'https://claw.nulong.me'},
  { title:'演算法實作', url:'https://algohw.nulong.me'},
  { title:'資訊安全報告',url:'https://docs.google.com/presentation/d/1ZT_rJsx_MY7aAh1CbTyb_rijOhRLJXgyOdsfAqHTCB4/edit?usp=sharing'},
  // { title:'CPE題目報告',url:'https://docs.google.com/presentation/d/1aqgiSEG9RRv5k29lRxyjP3roBLaLa3brzXYTzVBAThI/edit?usp=sharing'}
  // { title:'國家與市場 - 主持人投影片', url:'https://docs.google.com/presentation/d/103EdDxqWLoLa2F6ocIBfpbboU1zC9fEnAT3-yeF-Mwc/edit?usp=sharing'}
  , { title:'亞太投顧企劃',url:'https://hackmd.io/qNUcRMMESl-3AEOdPKtrzA'}
  , { title:'2023銘傳APCS夏令營',url:'https://docs.google.com/presentation/d/1cSRUGbOiRrtiRK8Z2CkVISHStgzdEokm5sEb8Vk6SY4/edit?usp=sharing'}
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
