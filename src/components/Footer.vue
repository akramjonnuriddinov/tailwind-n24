<template>
  <footer class="text-white bg-footer-bg">
    <div class="container px-5 py-8 mx-auto">
      <a class="flex mb-4" href="#">
        <img src="../assets/footer-logo.svg" alt="">
      </a>
      <div class="flex items-start justify-between border-b pb-7">
        <p class="w-56 text-xs font-normal leading-5">Воспроизводство, копирование, использование информации с сайта «NAMANGANLIKLAR24.UZ» возможно только с предварительного письменного разрешения редакции.</p>
        <ul>
          <li class="mb-5 last:mb-0" v-for="link1 in links1">
            <a class="font-medium leading-5 font-base hover:underline" href="#">{{ link1.text }}</a>
          </li>
        </ul>
        <ul>
          <li class="mb-5 last:mb-0" v-for="link2 in links2">
            <a class="font-medium leading-5 font-base hover:underline" href="#">{{ link2.text }}</a>
          </li>
        </ul>
      </div>
      <div class="flex items-start justify-between pt-5 pb-10">
        <p class="text-lg font-medium leading-6">Наши <br> социальные сети</p>
        <ul class="flex">
          <li class="mr-6">
            <a class="w-6 hover:opacity-80 active:opacity-60" href="#">
              <img src="../assets/network-icon/facebook.svg" alt="">
            </a>
          </li>
          <li class="mr-6">
            <a class="w-6 hover:opacity-80 active:opacity-60" href="#">
              <img src="../assets/network-icon/instagram.svg" alt="">
            </a>
          </li>
          <li class="mr-6">
            <a class="w-6 hover:opacity-80 active:opacity-60" href="#">
              <img src="../assets/network-icon/telegram.svg" alt="">
            </a>
          </li>
          <li>
            <a class="w-6 hover:opacity-80 active:opacity-60" href="#">
              <img src="../assets/network-icon/youtube.svg" alt="">
            </a>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      links1: [
        {id: 0, text: 'Информация о сайте'},
        {id: 1, text: 'Напишите нам'},
        {id: 2, text: 'Реклама'},
        {id: 3, text: 'Прислать новость'}
      ],
      links2: [
        {id: 0, text: 'Использование материалов'},
        {id: 1, text: 'Темы дня'},
        {id: 2, text: 'Наша команда'}
      ]
    }
  }
}
</script>