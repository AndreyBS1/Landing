<template>
  <div id="app">
    <intro></intro>
    <header>
      <b-navbar class='navbar'>
        <div class='project-name'>L A N D I N G</div>
      </b-navbar>
    </header>
    <main>
      <section class="info-section">
        <div class='text-section'>
          <h2 class='title'>BIG TEXT</h2>
          <p class='text'>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. 
            Maecenas id mauris vel leo congue semper. Suspendisse malesuada 
            eu metus mattis hendrerit. Aenean rutrum in erat et tincidunt. 
            Nulla ac ipsum placerat, pulvinar ligula at, tristique turpis. 
            In ut tellus at metus venenatis cursus.
          </p>
          </div>
        <div class='image-section'>
          <img src="./assets/logo.png" alt="IMAGE">
        </div>
      </section>
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
  font-family: cursive;
  margin: 0;
  padding: 0;
  color: snow;
  text-shadow:  black 1px 1px 1px;
}

header {
  font-size: 110%;
  padding: 0.7% 2%;
  background-color: #e27d60;
}

main {
  display: flex;
  flex-direction: row;
  justify-content: center;
  background-color: #41b3a3;
}

.info-section {
  width: 70vw;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 5% 3%;
  margin: 5% 0;
  background-color: #e8a87c;
  border: 20px solid #c38d9e;
  border-radius: 70px 20px;
  box-shadow: 10px 10px 3px #85dcb8;
}

.text-section {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  margin-right: 5px;
  width: 45%;
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
  margin-left: 5px;
  width: 45%;
  background-size: cover;
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
