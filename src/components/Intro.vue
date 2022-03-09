<template>
    <div class="intro">
        <div class="background-prism">
            <div class="welcome-text">
                <h1>РЕЗЮМЕ</h1>
                <h6>Автор: Бабенков Андрей</h6>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Intro',
}
</script>

<style scoped>
.intro {
    height: 100vh;
    background: no-repeat center / cover url(../assets/background_1.jpg);
}

.background-prism {
    width: 100%;
    height: 100%;
    background: linear-gradient(to right, rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.8));
}

.welcome-text {
    width: 100%;
    height: 100%;
    padding: 10%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-end;
    color: whitesmoke;
}
</style>
