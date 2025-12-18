
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

header h1 {
    font-size: 3em;
    margin: 0 0 10px;
    color: #fff;
    text-shadow: 2px 2px #ff69b4;
    animation: glow 2s infinite alternate;
}

header p {
    font-size: 1.2em;
    color: #fff;
    text-shadow: 1px 1px #ff69b4;
}

/* Мерцание заголовков */
@keyframes glow {
    0% { text-shadow: 2px 2px #ff69b4; color: #fff; }
    50% { text-shadow: 4px 4px #ff1493; color: #fff; }
    100% { text-shadow: 2px 2px #ff69b4; color: #fff; }
}

section {
    max-width: 800px;
    margin: 30px auto;
    background: rgba(255, 255, 255, 0.9);
    padding: 25px 30px;
    border-radius: 20px;
    box-shadow: 0 5px 20px rgba(0,0,0,0.2);
    opacity: 0;
    transform: translateY(20px);
    transition: opacity 1s ease, transform 1s ease;
}

section.visible {
    opacity: 1;
    transform: translateY(0);
}

section h2 {
    color: #ff1493;
    margin-bottom: 15px;
    font-size: 2em;
    text-align: center;
    animation: glow 2s infinite alternate;
}

section p {
    line-height: 1.6;
    font-size: 1.1em;
}

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
    transition: transform 0.5s ease, box-shadow 0.3s ease;
}

.button:hover {
    transform: translateY(-5px) rotate(-2deg) scale(1.05);
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
    <p>ЗА СЕБЯ голосовать нельзя (очевидно). Также наши катки будет комментировать секретный гость, который совсем ничего не понимает в игре и играл один раз в жизни, он также будет оценивать нашу игру и выставлять предварительный рейтинг самых крутых игроков (конечный выбор фаворита остается также за зрителем). Если количество симпатий у нескольких игроков совпадает, мы попросим каждого претендента рассказать нам новогодний стих/спеть новогоднюю песню в ДС канале!</p>
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

// Анимация секций при прокрутке
const sections = document.querySelectorAll('section');
function checkSections() {
    const triggerBottom = window.innerHeight * 0.85;
    sections.forEach(section => {
        const sectionTop = section.getBoundingClientRect().top;
        if(sectionTop < triggerBottom){
            section.classList.add('visible');
        }
    });
}
window.addEventListener('scroll', checkSections);
window.addEventListener('load', checkSections);
</script>

</body>
</html>
