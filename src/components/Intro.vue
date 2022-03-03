<template>
    <div v-show="intro" class="intro">
        <div
            class="welcome-text"
            v-show="firstWelcomeText"
            @click="clickOnFirstWelcomeText()"
        >
            <h1>Добро пожаловать!</h1>
            <h4>Тыкните куда-нибудь</h4>
        </div>
        <div
            class="welcome-text"
            v-show="secondWelcomeText"
            @click="clickOnSecondWelcomeText()"
        >
            <h1>
                Решил вот сделать себе лендинг =D
            </h1>
        </div>
        <div
            class="welcome-text"
            v-show="thirdWelcomeText"
            @click="clickOnThirdWelcomeText()"
        >
            <h1>
                Думаю, это будет нагляднее, чем слова в резюме.
            </h1>
        </div>
        <div
            class="welcome-text"
            v-show="fourthWelcomeText"
            @click="clickOnFourthWelcomeText()"
        >
            <h1>
                Ссылки на мои проекты Вы найдете в конце страницы.
            </h1>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Intro',
    data() {
        return {
            intro: true,
            firstWelcomeText: true,
            secondWelcomeText: false,
            thirdWelcomeText: false,
            fourthWelcomeText: false,
        }
    },
    methods: {
        clickOnFirstWelcomeText() {
            this.firstWelcomeText = false;
            this.secondWelcomeText = true;
        },
        clickOnSecondWelcomeText() {
            this.secondWelcomeText = false;
            this.thirdWelcomeText = true;
        },
        clickOnThirdWelcomeText() {
            this.thirdWelcomeText = false;
            this.fourthWelcomeText = true;
        },
        clickOnFourthWelcomeText() {
            this.fourthWelcomeText = false;
            this.intro = false;
        }
    }
}
</script>

<style scoped>
.intro {
    height: 100vh;
    background-color: #85c8b8;
}

.welcome-text {
    width: 100%;
    height: 100%;
    padding: 3%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    font-size: 5%;
}
</style>
