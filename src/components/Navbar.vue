<template>
  <div class="container px-5 pt-1 mx-auto mb-8">
    <nav class="pt-5 pb-5 border-b border-gray-300">
      <ul class="flex items-center justify-between">
        <li class="mr-[34px] last:mr-0" v-for="link in links">
          <a class="text-lg font-medium text-gray-500 capitalize" href="#">{{ link.text }}</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      links: [
        {id: 0, text: 'Главное'},
        {id: 1, text: 'Интересное'},
        {id: 2, text: 'Экономика'},
        {id: 3, text: 'Политика'},
        {id: 4, text: 'Общество'},
        {id: 5, text: 'Технологии'},
        {id: 6, text: 'Спорт'},
        {id: 7, text: 'Культура'},
        {id: 8, text: 'Происшествия'},
        {id: 9, text: 'Наука'}
      ]
    }
  }
}

</script>