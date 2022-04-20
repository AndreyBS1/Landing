<template>
  <div id="app">
    <intro-view />
  </div>
  <!-- <div id="app">
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
          <img src="./assets/img-1.jpg" alt="IMAGE">
        </div>
      </div>
      <div class="info-section even-section">
        <div class='image-section left-image'>
          <img src="./assets/logo.png" alt="IMAGE">
        </div>
        <div class='text-section right-text'>
          <h2 class='title'>Frontend</h2>
          <p class='text'>
            Почти все мои проекты написаны на Vue.js, 
            хотя немного умею и в React. Собственно, я 
            начинал программировать с фронта, поэтому в 
            этой области знаю немного больше.
          </p>
        </div>
      </div>
      <div class="info-section odd-section">
        <div class='text-section left-text'>
          <h2 class='title'>Backend</h2>
          <p class='text'>
            Бэк я обычно пишу на Node.js + Sequelize, в 
            качестве БД использую Postgres. Также работал 
            над сервером Python + Flask.
          </p>
        </div>
        <div class='image-section right-image'>
          <img src="./assets/node-logo.png" alt="IMAGE">
        </div>
      </div>
    </main>
    <contacts/>
  </div> -->
</template>

<script>
// import Intro from './components/Intro.vue'
// import Contacts from './components/Contacts.vue'
import IntroView from "@/views/IntroView";

export default {
  name: "App",
  components: {
    // Intro,
    // Contacts,
    IntroView,
  },
};
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

.odd-section {
  background-color: whitesmoke;
}

.even-section {
  background-color: #e6e6e6;
}

.text-section {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  width: 45%;
}

.left-text {
  margin-right: 5px;
}

.right-text {
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

.right-image {
  margin-left: 5px;
}

.left-image {
  margin-right: 5px;
}

img {
  width: 70%;
  border-radius: 10%;
}

footer {
  background-color: wheat;
  color: black;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  font-size: 120%;
}
</style>
