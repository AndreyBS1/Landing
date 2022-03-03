<template>
  <div id="app">
    <intro></intro>
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
  font-family: "Rany", sans-serif;
  margin: 0;
  padding: 0;
  color: #1b1d1c;
}

main {
  display: flex;
  flex-direction: row;
  justify-content: center;
  background-color: whitesmoke;
}

.info-section {
  width: 100vw;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10% 6%;
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
