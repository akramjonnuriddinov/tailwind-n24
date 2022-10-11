<template>
  <div class="container px-5 mx-auto mb-10">
    <div class="flex flex-wrap justify-between -mb-2">
      <div class="w-[394px] mr-[10px] last:mr-0 bg-zinc-100 mb-2 flex flex-col items-baseline justify-between rounded-[15px] px-[17px] pt-5 pb-[15px]" v-for="card in cards" :key="card">
        <h3 class="text-black font-medium mb-[10px] text-xl leading-[26px]">{{ card.title }}</h3>
        <p class="text-gray-600 font-base leading-[22px]">{{ card.text }}</p>
        <img class="my-[15px]" src="../assets/image-1.jpg" alt="">
        <div class="flex items-center">
          <img class="mr-[10px]" src="../assets/icon/icon-1.jpg" alt="">
          <span>{{ card.time }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      cards: [
        {id: 0, title: 'Кандидат на пост канцлера ФРГ Шольц назвал условия коалиционного соглашения', text: 'Лидер Социал-демократической партии Германии (СДПГ) и кандидат на должность...', img: 'image-1.jpg', time: 'ИА Красная Весна 15:55'},

        {id: 1, title: 'Ученые доказали экспериментальным путем пользу покровных культур', text: 'Новое исследование ученых университета Иллинойса объединяет полевые данные... ', img: 'image-1.jpg', time: 'Газета.Ru 12:54'},
        
        {id: 2, title: 'Baidu запустила публичный сервис роботакси Apollo Go в Шанхае', text: 'Автопарк Baidu состоит из модифицированных электромобилей EV... ', img: 'image-1.jpg', time: 'Хайтек+ 13:44'},
        
        {id: 3, title: 'Стали известны ёмкости аккумуляторов всех моделей iPhone 13', text: 'Во время презентации iPhone 13 Apple придала большое значения...', img: 'image-1.jpg', time: 'Digger.ru 14:25'},
        
        {id: 4, title: 'Nature: ученые смогли доказать природное происхождение коронавируса SARS-CoV-2', text: 'Во время презентации iPhone 13 Apple придала большое значение...', img: 'image-1.jpg', time: 'Lenta.ru 10:54'},
        
        {id: 5, title: 'Китайская марка JAC повысила цены на лифтбек и пикап в России', text: 'Две модели китайского бренда JAC из пяти, представленных на российском...', img: 'image-1.jpg', time: 'Тарантас Ньюс 10:44'}
      ]
    }
  }
}
</script>