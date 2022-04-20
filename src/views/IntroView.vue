<template>
  <div class="intro">
    <div class="background position"></div>
    <div class="wrapper position">
      <div class="text-wrapper">
        <h1>Babenkov Andrey</h1>
        <div class="line"></div>
        <h2>web developer</h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "IntroView",
};
</script>

<style scoped>
.intro {
  width: 100vw;
  height: 100vh;
  color: whitesmoke;
}

.position {
  width: 100%;
  height: 100%;
  position: absolute;
  left: 0;
  top: 0;
  bottom: 0;
  right: 0;
}

.background {
  background: no-repeat center / cover url(../assets/background_1.jpg);
  filter: blur(6px);
}

.wrapper {
  background-color: rgba(0, 0, 0, 0.7);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.text-wrapper {
  display: flex;
  flex-direction: column;
  align-items: flex-end;
}

h1 {
  margin-bottom: 5px;
}

h2 {
  margin-top: 5px;
}

.line {
  width: 50%;
  height: 3px;
  background-color: #e54b4b;
}
</style>
