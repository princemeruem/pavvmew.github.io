
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Кастомная игра с pavvmew | Dead By Daylight</title>

<!-- Шрифт -->
<link href="https://fonts.googleapis.com/css2?family=Indie+Flower&display=swap" rel="stylesheet">

<style>
/* ===== ОСНОВА ===== */
body {
    margin: 0;
    font-family: 'Indie Flower', cursive;
    background: linear-gradient(180deg, #fff0f5 0%, #ffb6c1 100%);
    color: #333;
    overflow-x: hidden;
}

/* ===== ШАПКА ===== */
header {
    text-align: center;
    padding: 50px 20px 30px;
}

header h1 {
    font-size: 3em;
    margin-bottom: 10px;
    color: #ffffff;
    text-shadow: 2px 2px 0 #ff69b4;
}

header p {
    font-size: 1.3em;
    color: #ffffff;
    text-shadow: 1px 1px 0 #ff69b4;
}

/* ===== КОНТЕНТНЫЕ БЛОКИ ===== */
section {
    max-width: 850px;
    margin: 30px auto;
    background: rgba(255, 255, 255, 0.92);
    padding: 30px;
    border-radius: 25px;
    box-shadow: 0 10px 30px rgba(255,105,180,0.25);
}

section h2,
.features h3,
.gifts h3,
.rewards h3 {
    text-align: center;
    color: #ff1493;
    margin-bottom: 20px;
    font-size: 2em;
}

section p {
    font-size: 1.25em;
    line-height: 1.6;
    margin-bottom: 15px;
}

/* ===== ПОДЧЕРКИВАНИЯ ===== */
.underline {
    text-decoration: underline;
}

/* ===== КНОПКИ ===== */
.button {
    display: inline-block;
    margin: 10px;
    padding: 12px 22px;
    background: #ffffff;
    color: #ff69b4;
    border-radius: 16px;
    text-decoration: none;
    font-size: 1.2em;
    box-shadow: 0 6px 15px rgba(255,105,180,0.35);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.button:hover {
    transform: translateY(-4px) scale(1.05);
    box-shadow: 0 10px 25px rgba(255,105,180,0.45);
}

/* ===== СПЕЦ БЛОКИ ===== */
.features,
.gifts,
.rewards {
    background: rgba(255, 255, 255, 0.95);
}

/* ===== СНЕГ ===== */
.snowflake {
    position: fixed;
    top: -20px;
    color: #ffffff;
    font-size: 1em;
    pointer-events: none;
    animation: fall linear infinite;
    z-index: 9999;
}

@keyframes fall {
    from { transform: translateY(-20px); }
    to { transform: translateY(110vh); }
}
</style>
</head>

<body>

<header>
    <h1>Кастомная игра с pavvmew</h1>
    <p>Dead By Daylight · 25.12.2025 · Формат 4v1</p>
</header>

<section>
    <h2>Правила</h2>

    <p>
        Твоя задача сегодня — завоевать как можно больше зрительских симпатий!
        Они смогут проголосовать за тебя, отдав свои баллы канала в твой новогодний подарок ;)
    </p>

    <p>
        Собирай свой оригинальный новогодний лук в лобби, кидайся снежками,
        авантюрно отбегай злого деда Мороза 5 генераторов,
        тибагай, кивай, тверкай в паллетах,
        но не забывай спасти как можно больше товарищей.
    </p>

    <p>
        После игры за сурвов стороны меняются, и ты обязательно будешь злым дедом Морозом.
        Здесь твоя задача — проявить креативность
        (необычные и забавные билды, редкие маны, странные тактики)
        и наказать минимум трёх непослушных оленей.
    </p>

    <p>
        Я играю вместе с вами за обе стороны, поэтому чаще попадайся на глаза —
        так твои шалости точно будут замечены.
    </p>

    <p>
        По окончанию матчей мы подсчитаем количество симпатий и определим победителя!
    </p>

    <p>
        Также ты можешь участвовать в активности
        <span class="underline">«лучший чаттерс»</span> —
        делай клипы, шути, комментируй и проявляй активность.
    </p>
</section>

<section class="features">
    <h3>Особенности</h3>

    <p>
        Наши игры будет комментировать
        <span class="underline">новогодний кролик</span>,
        который ничего не понимает в игре и создаёт атмосферу веселья.
    </p>

    <p>
        За <span class="underline">СЕБЯ</span> голосовать нельзя :Р
    </p>

    <p>
        При равенстве симпатий участники читают
        <span class="underline">новогодний стих</span>
        или <span class="underline">поют песню</span>.
    </p>
</section>

<section class="gifts">
    <h3>Подарки от pavvmew</h3>

    <p>
        Победитель получает милый брелок с котиком,
        лапку-сквиш и ручную открытку.
        Отправка по РФ, для других регионов — мини-арт от меня &lt;3
    </p>
</section>

<section class="rewards">
    <h3>Награды за баллы канала</h3>

    <p>100 лапок — симпатия игроку</p>
    <p>Минимум 100, максимум 3000 лапок на одного игрока</p>
</section>

<section style="text-align:center;">
    <h2>Соцсети</h2>
    <a class="button" href="https://t.me/pavvmew" target="_blank">Telegram</a>
    <a class="button" href="https://www.tiktok.com/@pavvmi?_t=ZS-8zD1VOxHDUn&_r=1" target="_blank">TikTok</a>
    <a class="button" href="https://steamcommunity.com/id/pavvmi/" target="_blank">Steam</a>
</section>

<script>
function createSnowflake() {
    const snow = document.createElement("div");
    snow.className = "snowflake";
    snow.textContent = "❄";
    snow.style.left = Math.random() * window.innerWidth + "px";
    snow.style.fontSize = (Math.random() * 20 + 10) + "px";
    snow.style.animationDuration = (Math.random() * 5 + 5) + "s";
    document.body.appendChild(snow);
    setTimeout(() => snow.remove(), 10000);
}
setInterval(createSnowflake, 200);
</script>

</body>
</html>
