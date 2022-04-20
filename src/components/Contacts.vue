<template>
    <div class="contacts">
        <div class="contacts-header">
            <h2>Ссылки на мои проекты</h2>
        </div>
        <div class="contacts-text">
            <h4><a href="https://github.com/AndreyBS1">Github</a></h4>
        </div>
        <div class="contacts-text">
            <h4><a href="https://noteskeeperappl.herokuapp.com/">Noteskeeper</a></h4>
            <h6 class="comment" align="justify">
                <i>
                    Бесплатный сервер уходит в спящий режим, когда 
                    на него не приходят запросы; на включение нужно 
                    несколько секунд. Попробуйте обновить страницу 
                    несколько раз.
                </i>
            </h6>
        </div>
        <div>
            <h4><a href="https://t.me/MusicTransfer_Bot">Телеграм бот для трансфера музыки</a></h4>
        </div>
        <div class="contacts-header">
            <h2>Мои контакты</h2>
        </div>
        <div class="contacts-text">
            <h4>Телефон: +7 909 592 5995</h4>
        </div>
        <div class="contacts-text">
            <h4>Почта: andrey.babenkov.00@gmail.com</h4>
        </div>
        <div class="contacts-text">
            <h4><a href="https://t.me/andreybs1">Телеграм</a></h4>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Contacts',
}
</script>

<style scoped>
.contacts {
    height: 100vh;
    background: no-repeat center / cover url(../assets/background_2.jpg);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    color: black;
}

.contacts-header {
    margin: 1% 0;
}

.contacts-text {
    margin: 0.5% 0;
    max-width: 50vw;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

a {
    outline: none;
    text-decoration: none;
    padding: 10px;
    border-radius: 5%;
}

a:link {
    color: black;
}

a:visited {
    color: black;
}

a:focus {
    border-bottom: medium solid brown;
    background-color: wheat;
}

a:hover {
    border-bottom: medium solid red;
    background-color: whitesmoke;
}

a:active {
    color: black;
}

.comment {
    margin: 2% 0;
}
</style>
