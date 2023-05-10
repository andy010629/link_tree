<template>
  <div @click="link_to(props.url)" style="cursor: pointer;" class="hover:opacity-90 hover:-translate-y-2 duration-300 p-6 px-4  text-xl font-bold  bg-slate-300 shadow rounded-lg shadow-slate-100">
    <div class="text-gray-800 select-none hover:text-gray-700 w-full"  :href="props.url" target="_blank">{{ props.title }}</div>
</div>
</template>

<script setup lang="ts">
import { defineProps } from 'vue'
const props = defineProps({
  title: String,
  url: String,
})

function link_to(url: string | undefined) {
  if (url) {
    window.open(url, '_blank');
  }
}


</script>

<style scoped>

</style>