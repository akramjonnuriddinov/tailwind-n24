<script setup>
import Button from './Button.vue'
</script>

<template>
  <section>
    <div class="notification container rounded-[10px] px-5 mx-auto max-w-[1090px] mb-[60px] py-6 pl-[29px] pr-[71px] flex justify-between items-center">
      <h2 class="max-w-[404px] w-full text-black font-medium text-xl leading-[26px] mr-4">
        Хотите быть в курсе свежих новостей?  Включите уведомления!
      </h2>
      <Button class="bg-orange-400 px-[30px] py-[13px] text-xl leading-[23.7px]" name="Включит" />
    </div>
  </section>
</template>

<style scoped>
.notification {
  background-image: url('../assets/notification-bg.jpg');
  background-repeat: no-repeat;
  background-size: cover;
}
</style>