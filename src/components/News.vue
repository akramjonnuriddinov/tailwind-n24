<template>
  <section>
    <div class="container px-5 mx-auto">
      <h2 class="font-medium mb-5 text-black text-2xl leading-[28.44px]">В мире</h2>
      <div class="flex justify-between">
        <ul class="mr-[10px]">
          <li class="bg-zinc-100 max-w-[797px] rounded-[15px] w-full flex py-5 pl-[17px] pr-5 mb-[10px] last:mb-0" v-for="card in cards">
            <img class="mr-[15px]" src="../assets/image-2.jpg" alt="" width="210" height="165">
            <div>
              <h3 class="mb-[10px]">
                <a class="font-medium hover:underline text-black text-xl leading-[26px]" href="#">{{ card.title }}</a>
              </h3>
              <p class="text-[#4A4B4C] font-base leading-[22px] mb-[17px]">{{ card.text }}</p>
              <div class="flex items-center span">
                <img class="mr-[10px]" src="../assets/icon/icon-2.jpg" alt="">
                <span>{{ card.time }}</span>
              </div>
            </div>
          </li>
        </ul>
        <div class="max-w-[393px] flex flex-col justify-between w-full">
          <div class="px-[17px] mb-[10px] pt-5 pb-[25px] bg-zinc-100 rounded-[15px]">
            <h3 class="text-2xl font-medium text-black leading-[28.44px] mb-[25px]">Главное</h3>
            <ul>
              <li class="pb-5 border-b border-[rgb(210,210,210)] last:border-none last:pb-0 pt-5 first:pt-0 flex flex-col" v-for="item in news">
                <a class="mb-2 text-lg font-medium leading-6 text-black hover:underline" href="#">{{ item.link }}</a>
                <span class="text-[#5E5F61] text-[13px] leading-[15.41px] font-normal">{{ item.time }}</span>
              </li>
            </ul>
          </div>
          <a href="#">
            <img class="h-[338px] rounded-[15px] object-cover" src="../assets/image-3.jpg" width="393" height="338" alt="">
          </a>
        </div>
      </div>
      <a class="bg-[#EAEAEA] px-5 py-[17px] mt-[17px] rounded-[10px] mb-[100px] flex items-center justify-center max-w-[796px] w-full text-black hover:opacity-80 active:opacity-60" href="#">Показать ещё</a>
    </div>
  </section>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      cards: [
        {id: 0, title: 'Китайский Чунцин запустил чартерный рейс для студентов до Британии', text: 'Чартерный рейс с 244 китайскими студентами вылетел из города центрального подчинения Чунцина на юго-западе Китая в британский Манчестер...', time: 'ИА Красная Весна 12:25'},
        
        {id: 1, title: 'В Германии выпустят ограниченную партию плюшевых мишек в образе Меркель', text: 'БЕРЛИН, 19 сентября. / ТАСС/. Знаменитая фабрика по производству плюшевых игрушек в городе Кобург (федеральная земля Бавария) изготовила уникального...', time: 'ТАСС 11:35'},
        
        {id: 2, title: 'Акции КНР утратили доверие инвесторов. Что делать с бумагами прямо сейчас', text: 'За последние месяцы инвесторы в китайский рынок пережили настоящее потрясение — из-за ужесточения регулирования технологического сектора и критики некоторых...', time: 'РБК Инвестиции 09:35'},

        {id: 3, title: 'Китай раскритиковал заключенный Австралией, США и Великобританией антикитайский союз AUKUS', text: 'Не только Франция, которая лишилась многомиллиардного контракта с Австралий, осталась недовольна созданием трехстороннего оборонного альянса AUKUS, пишет Anna-News.info', time: 'Solenka.info 19:43'}
      ],
      news: [
        {id: 0, link: 'В Фергане создадут узбекско-пакистанский университет', time: 'Sputnik Узбекистан 14:09'},
        {id: 1, link: 'Узбекистан утвердил соглашение о содействии занятости в странах СНГ', time: 'ИА Красная Весна 10:19'},
        {id: 2, link: 'В Узбекистане увеличиваются очереди за автомобилями UzAuto', time: 'Северная газета (Армянск) 13:50'},
        {id: 3, link: 'Минтуризма опровергло приостановку выплат за шаги', time: 'Sputnik Узбекистан 14:32'}
      ]
    }
  }

}
</script>