
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Кастомная игра с pavvmew | Dead By Daylight</title>
<link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">
<style>
body {
    margin: 0;
    font-family: 'Pacifico', cursive;
    background: #ffb6c1; /* розовый фон */
    color: #333;
    overflow-x: hidden;
    position: relative;
}

header {
    text-align: center;
    padding: 50px 20px;
}

header h1, header p {
    position: relative;
}

section {
    max-width: 800px;
    margin: 30px auto;
    background: rgba(255, 255, 255, 0.9);
    padding: 25px 30px;
    border-radius: 20px;
    box-shadow: 0 5px 20px rgba(0,0,0,0.2);
    position: relative;
}

/* Снеговые сугробы сверху заголовков и секций */
header h1::before,
header p::before,
section h2::before {
    content: "";
    position: absolute;
    top: -10px;
    left: 0;
    width: 100%;
    height: 20px;
    background: url('data:image/svg+xml;utf8,<svg width="100%" height="20" xmlns="http://www.w3.org/2000/svg"><ellipse cx="10" cy="10" rx="10" ry="5" fill="white"/><ellipse cx="30" cy="10" rx="12" ry="6" fill="white"/><ellipse cx="60" cy="10" rx="8" ry="4" fill="white"/><ellipse cx="90" cy="10" rx="15" ry="7" fill="white"/></svg>') repeat-x;
    background-size: auto 20px;
}

/* Заголовки */
section h2 {
    color: #ff1493;
    margin-bottom: 15px;
    font-size: 2em;
    text-align: center;
    padding-top: 10px;
}

/* Параграфы */
section p {
    line-height: 1.6;
    font-size: 1.1em;
}

/* Кнопки */
.button {
    display: inline-block;
    padding: 12px 20px;
    margin: 10px 5px 0 0;
    background: #fff;
    color: #ff69b4;
    font-weight: bold;
    border-radius: 12px;
    text-decoration: none;
    box-shadow: 0 4px 10px rgba(0,0,0,0.2);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.button:hover {
    transform: translateY(-5px) scale(1.05);
    box-shadow: 0 8px 15px rgba(0,0,0,0.3);
}

/* Снег */
.snowflake {
    position: fixed;
    top: -10px;
    color: #fff;
    font-size: 1em;
    user-select: none;
    z-index: 9999;
    pointer-events: none;
    animation-name: fall;
    animation-timing-function: linear;
    animation-iteration-count: infinite;
}

@keyframes fall {
    0% { transform: translateY(-10px); }
    100% { transform: translateY(100vh); }
}
</style>
</head>
<body>

<header>
    <h1>Кастомная игра с pavvmew</h1>
    <p>Dead By Daylight | 25.12.2025 | Формат 4v1</p>
</header>

<section>
    <h2>Правила</h2>
    <p>Твоя задача завоевать как можно больше зрительских симпатий!! Они смогут проголосовать за тебя, отдав свои баллы канала в твою новогоднюю коробочку ;) Собери интересный новогодний лук своему сурву, кидайся снежками, манси 5 генов, развесели зрителя своей игрой, при этом ты должен выиграть и спасти как можно больше товарищей.</p>
    <p>После игры за сурвов стороны меняются и ты обязательно будешь киллером, здесь твоя задача быть оригинальным (пробуй разные билды, манов, тактики) и сделать -3. По окончанию матчей мы подсчитаем количество заработанных симпатий (баллов канала) и отправим символический подарочек победителю почтой (вы должны проживать в РФ), если вы живете в другом месте, подарок будет цифровой :р.</p>
    <p>ЗА СЕБЯ голосовать нельзя (очевидно). Также наши катки будет комментировать секретный гость, который совсем ничего не понимает в игре и играл один раз в жизни, он также будет оценивать нашу игру и выставить предварительный рейтинг самых крутых игроков (конечный выбор фаворита остается также за зрителем). Если количество симпатий у нескольких игроков совпадает, мы попросим каждого претендента рассказать нам новогодний стих/спеть новогоднюю песню в ДС канале!</p>
    <p>Это еще не все, пока остальные веселят тебя в игре, ты можешь также поучаствовать в активности "лучший чаттерс" — делай забавные клипы, оригинально шути и комментируй происходящее, заливай свои баллы канала и активно проявляй себя. В конце стрима я и модератор определят победителя и отправим ему маленький подарок! (если вы также играете с нами в кастомке, есть возможность залутать несколько наград)</p>
</section>

<section style="text-align:center;">
    <h2>Соцсети</h2>
    <a class="button" href="https://t.me/pavvmew" target="_blank">Telegram</a>
    <a class="button" href="https://www.tiktok.com/@pavvmi?_t=ZS-8zD1VOxHDUn&_r=1" target="_blank">TikTok</a>
    <a class="button" href="https://steamcommunity.com/id/pavvmi/" target="_blank">Steam</a>
</section>

<script>
// Снег
function createSnowflake() {
    const snowflake = document.createElement('div');
    snowflake.classList.add('snowflake');
    snowflake.textContent = '❄';
    snowflake.style.left = Math.random() * window.innerWidth + 'px';
    snowflake.style.fontSize = (Math.random()*25 + 10) + 'px';
    snowflake.style.animationDuration = (Math.random()*5 + 5) + 's';
    document.body.appendChild(snowflake);
    setTimeout(() => snowflake.remove(), 10000);
}
setInterval(createSnowflake, 200);
</script>

</body>
</html>
