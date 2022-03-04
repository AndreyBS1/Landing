<template>
  <div id="app">
    <intro></intro>
    <main>
      <div class="info-section odd-section">
        <div class='text-section left-text'>
          <h2 class='title'>Что, зачем и почему?</h2>
          <p class='text'>
            Я подумал, что резюме в формате Word выглядит неубедительно.
            Поэтому появился этот небольшой сайт - тут я буду выкладывать
            ссылки на свои проекты, описывать свои навыки и прочее, прочее...
          </p>
        </div>
        <div class='image-section right-image'>
          <img src="./assets/logo.png" alt="IMAGE">
        </div>
      </div>
      <div class="info-section even-section">
        <div class='image-section left-image'>
          <img src="./assets/logo.png" alt="IMAGE">
        </div>
        <div class='text-section right-text'>
          <h2 class='title'>Основной стек</h2>
          <p class='text'>
            Сейчас я пишу на Vue + Node. Немножко
            умею в Python и PHP (собственно, изучаю их для 
            написания бэка). В качестве БД использую Postgres.
          </p>
        </div>
      </div>
      <div class="info-section odd-section">
        <div class='text-section left-text'>
          <h2 class='title'>BIG TEXT</h2>
          <p class='text'>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
            Maecenas id mauris vel leo congue semper. Suspendisse malesuada 
            eu metus mattis hendrerit. Aenean rutrum in erat et tincidunt. 
            Nulla ac ipsum placerat, pulvinar ligula at, tristique turpis. 
            In ut tellus at metus venenatis cursus.
          </p>
        </div>
        <div class='image-section right-image'>
          <img src="./assets/logo.png" alt="IMAGE">
        </div>
      </div>
    </main>
    <footer>
      <p>Some contact information</p>
    </footer>
  </div>
</template>

<script>
import Intro from './components/Intro.vue'

export default {
  name: 'App',
  components: {
    Intro,
  }
}
</script>

<style>
#app {
  font-family: "Rany", sans-serif;
  margin: 0;
  padding: 0;
  color: #1b1d1c;
}

main {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.info-section {
  height: 100vh;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10% 6%;
}

.odd-section{
  background-color: whitesmoke;
}

.even-section{
  background-color: #e6e6e6;
}

.text-section {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  width: 45%;
}

.left-text{
  margin-right: 5px;
}

.right-text{
  margin-left: 5px;
}

.title {
  font-size: 150%;
  font-weight: bold;
}

.text {
  text-align: justify;
  font-size: 150%;
  margin: 7% 0;
}

.image-section {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 45%;
  background-size: cover;
}

.right-image{
  margin-left: 5px;
}

.left-image{
  margin-right: 5px;
}

img {
  width: 70%;
}

footer {
  background-color: black;
  color: wheat;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100px;
  font-size: 120%;
}
</style>
