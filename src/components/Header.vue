<template>
  <header class="bg-zinc-100">
    <div class="container flex justify-between items-center mx-auto px-5 py-[30px]">
      <div class="flex items-center">
        <a class="mr-[35px]" href="#">
          <img src="../assets/logo.png" alt="Site logo">
        </a>
        <div class="text-base text-gray-600 leading-[19px]">
          <span class="mr-6">
            <span class="font-bold text-blue-600">$</span> 10137.2
          </span>
          <span>
            <span class="font-bold text-blue-600">P</span> 138.26
          </span>
        </div>
      </div>
      <div class="flex items-center">
        <input class="max-w-[275px] mr-6 w-full py-3 px-4 rounded-full" type="text" placeholder="Поиск">
        <div class="flex items-center p-1 mr-6 bg-blue-100 rounded-full">
          <a class="mr-2 text-black px-[7px] py-[9px] w-[30px] h-[30px] rounded-full bg-white flex items-center justify-center" href="#">УЗ</a>
          <a class="text-gray-400" href="#">РУ</a>
        </div>
        <Button name="Voyti" />
      </div>
    </div>
  </header>
</template>

<script setup>
import Button from './Button.vue'
</script>