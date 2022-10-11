<template>
  <Header />
  <main>
    <Navbar />
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
  components: {
    Header,
    Navbar,
    Card,
    Notification,
    News,
    Footer
  }
}

</script>

<style>

</style>
