
<template>
<div class="header bg-black bg-right bg-contain bg-no-repeat bg-hero">
<div class="w-full flex justify-between  p-1 px-7 position-static">
<div class="flex p-1 m-3 flex-row justify-center">
<logo />
<ul class="text-white block p-4 pl-10">
<NuxtLink v-for="{ link, title } in links" :key="link" :to="link">
  {{ title }}
</NuxtLink>
</ul>
</div>
<div class="button pt-4">
<button class=" bg-blue-900 border rounded text-white  h-10 w-40   m-3">Nous contacter</button>
</div>
</div>
<div class="main grid p-10" alig>
<img class="mb-5" src="../assets/images/Logo-MI-1.png" alt="">
<div id="solutions" class="content">
<h1 class="text-white text-5xl">Des solution adaptées</h1>
<h2 class="text-red-800 text-4xl">à vos besions</h2>
<p class="text-white text-2xl">Amin aute id magna aliqua ad ad non deserunt sunt. Qui irure qui lorem</p>
</div>
</div>
<div class="nos-valeurs grid sm:grid-cols-1 md:grid-cols-2 lg:grid-cols-3 sm:text-white md:text-blue-900 justify-around border-t-2 pt-5 pb-5 ">
  <div class="valeur-1 border rounded pb-2">
    <img  class="" src="../assets/images/logo-cic.jpeg" alt="">
   <h3 class=" text-center">Valeur 1</h3>
   <p class="text-center">Benoit, faut rédiger un potit text slp</p>
  </div>
  <div class="valeur-2 border rounded">
    <img  class="" src="../assets/images/logo-cic.jpeg" alt="">
    <h3 class="text-center">Valeur 1</h3>
    <p class="text-center">Benoit, faut rédiger un potit text slp</p>
  </div>
  <div id="values" class="valeur-3 border rounded">
    <img  class="" src="../assets/images/logo-cic.jpeg" alt="">
    <h3 class="text-center">Valeur 1</h3>
    <p class="text-center">Benoit, faut rédiger un potit text slp</p>
  </div>
</div>
</div>
</template>
<script>
import logo from '@/components/Logo'

export default {
  name: 'Hero',
  components: {
    logo
  },
  data () {
    return {
      links: [
        { link: '/#values', title: 'Nos valeurs' },
        { link: '/#solutions', title: 'Notre solutions' },
        { link: '/', title: 'Nos partenaire' },
        { link: '/', title: 'L\'équipe' },
        { link: '/', title: 'bloc' }
      ]
    }
  }
}</script>
