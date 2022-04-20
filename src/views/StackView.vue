<template>
  <div class="stack">
    <div class="wrapper tech-wrapper">
      <div class="tech left">
        <p class="primary">осн</p>
        <h2>Vue.js</h2>
      </div>
      <div class="tech right">
        <p class="primary">осн</p>
        <h2>Node.js</h2>
      </div>
    </div>
    <div class="wrapper text-wrapper">
      <div class="circle text-wrapper">
        <h1>Мой стек</h1>
      </div>
    </div>
    <div class="wrapper tech-wrapper">
      <div class="tech left">
        <p class="secondary">доп</p>
        <h2>React</h2>
      </div>
      <div class="tech right">
        <p class="secondary">доп</p>
        <h2>Python</h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "StackView",
};
</script>

<style scoped>
.stack {
  width: 100vw;
  height: 100vh;
  background-color: whitesmoke;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.wrapper {
  width: 100%;
  height: 30%;
  padding: 0 10%;
}

.text-wrapper {
  display: flex;
  justify-content: center;
  align-items: center;
}

.circle {
  width: 400px;
  height: 400px;
  border: solid 2px black;
  border-radius: 100%;
}

.tech-wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.tech {
  width: 30%;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.tech.left {
  align-items: flex-start;
}

.tech.right {
  align-items: flex-end;
}

.tech p {
  width: 30%;
  border-radius: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.primary {
  background-color: #61bfad;
}

.secondary {
  background-color: #eed974;
}
</style>
