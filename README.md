
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
}

header p {
    font-size: 1.2em;
    color: #fff;
    text-shadow: 1px 1px #ff69b4;
}

section {
    max-width: 800px;
    margin: 30px auto;
    background: rgba(255, 255, 255, 0.9);
    padding: 25px 30px;
    border-radius: 20px;
    box-shadow: 0 5px 20px rgba(0,0,0,0.2);
}

section h2 {
    color: #ff1493;
    margin-bottom: 15px;
    font-size: 2em;
    text-align: center;
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
    transition: transform 0.3s, box-shadow 0.3s;
}

.button:hover {
    transform: translateY(-3px);
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

/* Футер с елками и Санта-Клаусом */
.footer {
    position: relative;
    width: 100%;
    height: 250px;
    background: linear-gradient(to top, #ffb6c1 0%, #ffb6c1 70%, #fff0 100%);
    overflow: hidden;
}

/* Елки SVG */
.tree {
    position: absolute;
    bottom: 0;
    width: 60px;
    height: 120px;
}

.tree svg {
    width: 100%;
    height: 100%;
}

@keyframes twinkle {
    0%, 100% { fill: #fff; }
    50% { fill: #ff0; }
}

/* Санта-Клаус */
.santa {
    position: absolute;
    bottom: 150px;
    left: -250px;
    width: 250px;
    height: 120px;
    background: url('https://i.imgur.com/4J6hQjG.png') no-repeat;
    background-size: contain;
    animation: santaMove 20s linear infinite;
}

@keyframes santaMove {
    0% { left: -250px; }
    100% { left: 100%; }
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

<div class="footer">
    <!-- Елки с мерцающими огоньками -->
    <div class="tree" style="left:30px;">
        <svg viewBox="0 0 64 128">
            <polygon points="32,0 0,64 64,64" fill="green"/>
            <circle cx="16" cy="40" r="3" style="animation: twinkle 2s infinite;"></circle>
            <circle cx="48" cy="50" r="3" style="animation: twinkle 3s infinite;"></circle>
            <circle cx="32" cy="30" r="3" style="animation: twinkle 1.5s infinite;"></circle>
        </svg>
    </div>
    <div class="tree" style="left:120px;">
        <svg viewBox="0 0 64 128">
            <polygon points="32,0 0,64 64,64" fill="green"/>
            <circle cx="20" cy="35" r="3" style="animation: twinkle 2.5s infinite;"></circle>
            <circle cx="44" cy="45" r="3" style="animation: twinkle 1.8s infinite;"></circle>
        </svg>
    </div>
    <div class="tree" style="left:220px;">
        <svg viewBox="0 0 64 128">
            <polygon points="32,0 0,64 64,64" fill="green"/>
            <circle cx="16" cy="40" r="3" style="animation: twinkle 1.6s infinite;"></circle>
            <circle cx="48" cy="50" r="3" style="animation: twinkle 2.2s infinite;"></circle>
        </svg>
    </div>
    <div class="tree" style="left:320px;">
        <svg viewBox="0 0 64 128">
            <polygon points="32,0 0,64 64,64" fill="green"/>
            <circle cx="24" cy="38" r="3" style="animation: twinkle 2s infinite;"></circle>
        </svg>
    </div>
    <div class="tree" style="left:420px;">
        <svg viewBox="0 0 64 128">
            <polygon points="32,0 0,64 64,64" fill="green"/>
            <circle cx="32" cy="30" r="3" style="animation: twinkle 1.7s infinite;"></circle>
        </svg>
    </div>
    <!-- Санта -->
    <div class="santa"></div>
</div>

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
