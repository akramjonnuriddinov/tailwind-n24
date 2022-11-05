<template>
  <Header />
  <main>
    <div class="container px-5 pt-1 mx-auto mb-8">
    <nav class="pt-5 pb-5 border-b border-gray-300">
      <ul class="flex items-center justify-between">
        <li class="mr-[34px] last:mr-0">
          <routerLink to="/" class="text-lg font-medium text-gray-500 capitalize" >Главное</routerLink>
        </li>
        <li class="mr-[34px] last:mr-0">
          <routerLink to="/list" class="text-lg font-medium text-gray-500 capitalize" >Интересное</routerLink>
        </li>
        <li class="mr-[34px] last:mr-0">
          <a class="text-lg font-medium text-gray-500 capitalize" href="#">Экономика</a>
        </li>
        <li class="mr-[34px] last:mr-0">
          <a class="text-lg font-medium text-gray-500 capitalize" href="#">Политика</a>
        </li>
        <li class="mr-[34px] last:mr-0">
          <a class="text-lg font-medium text-gray-500 capitalize" href="#">Общество</a>
        </li>
        <li class="mr-[34px] last:mr-0">
          <a class="text-lg font-medium text-gray-500 capitalize" href="#">Технологии</a>
        </li>
        <li class="mr-[34px] last:mr-0">
          <a class="text-lg font-medium text-gray-500 capitalize" href="#">Спорт</a>
        </li>
        <li class="mr-[34px] last:mr-0">
          <a class="text-lg font-medium text-gray-500 capitalize" href="#">Культура</a>
        </li>
        <li class="mr-[34px] last:mr-0">
          <a class="text-lg font-medium text-gray-500 capitalize" href="#">Происшествия</a>
        </li>
        <li class="mr-[34px] last:mr-0">
          <a class="text-lg font-medium text-gray-500 capitalize" href="#">Наука</a>
        </li>
      </ul>
    </nav>
  </div>
    <div>
      <div class="container mx-auto px-5 mb-[50px]">
        <a class="w-full" href="#">
          <img class="w-full" src="./assets/adv.jpg" alt="">
        </a>
      </div>
    </div>
    <Card />
    <Notification />
    <News />
  </main>
  <Footer />
  <router-view/>
</template>

<script>
import Header from './components/Header'
import Navbar from './components/Navbar'
import Card from './components/Card'
import Notification from './components/Notification'
import News from './components/News'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: { Header, Navbar, Card, Notification, News, Footer }
}

</script>

<style>

</style>
