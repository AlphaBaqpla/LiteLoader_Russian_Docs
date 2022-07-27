---
home: true
sidebar: false
heroText:
tagline:
---

<div class="content">
    <div class="row">
        <div class="col-sm-3">
            <p class="logo_p"><img src="/assets/compass.png" alt="Logo"></p>
        </div>
        <div class="col-sm-9">
            <h1>Навигатор</h1>
            <p>Здесь вы найдете ссылки на <code>JavaScript/Lua/.NET/C++</code> документации</p>
        </div>
    </div>
    <div class="row buttons-content">
        <div class="col-sm-6 btn-link"><a href="/ru_RU/Usage" class="navigator-link">🔨 Установка и использование</a></div>
        <div class="col-sm-6 btn-link"><a href="/ru_RU/QA" class="navigator-link">❓ Известные баги</a></div>
        <div class="col-sm-6 btn-link"><a class="navigator-link">⛳ C++ Документация (скоро)</a></div>
        <div class="col-sm-6 btn-link"><a class="navigator-link">🪁 .NET Документация (скоро)</a></div>
        <div class="col-sm-6 btn-link"><a href="/ru_RU/Development" class="navigator-link">🎯 JavaScript/Lua Документация</a></div>
        <div class="col-sm-6 btn-link"><a href="/ru_RU/Maintenance" class="navigator-link">🎬 Разработка и обслуживание</a></div>
    </div>
</div>

<style>
.content {
    margin: 30px 0;
}

.logo_p {
    text-align: center;
}

.logo_p img {
    width: 128px;
    image-rendering: pixelated;
}

.btn-link {
    margin-top: 20px;
}

.navigator-link {
    border: 1px solid #3eaf7c;
    display: flex;
    padding: 16px;
    border-radius: 6px;
}

@media screen and (max-width: 576px) {
    .logo_p {
        text-align: left;
    }
}
</style>
