<script setup>
defineProps({
  name: String,
})
</script>

<template>
  <a class="bg-blue-400 text-white px-5 py-3 font-base font-medium rounded-[10px] leading-[18.96px]" href="#">{{ name }}</a>
</template>