
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Кастомная игра с pavvmew | Dead By Daylight</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap');

body {
    margin: 0;
    font-family: 'Montserrat', sans-serif;
    background: linear-gradient(to bottom, #ffffff, #ffe6f0);
    color: #333;
    overflow-x: hidden;
    position: relative;
}

header {
    text-align: center;
    padding: 50px 20px;
    background: rgba(255,255,255,0.6);
    position: relative;
    z-index: 2;
}

header h1 {
    font-size: 3em;
    margin: 0 0 10px 0;
    color: #ff69b4;
}

header p {
    font-size: 1.2em;
    color: #555;
}

.timer {
    text-align: center;
    font-size: 2em;
    margin: 20px 0;
    color: #ff69b4;
}

section {
    max-width: 800px;
    margin: 40px auto;
    background: rgba(255, 255, 255, 0.9);
    padding: 30px;
    border-radius: 15px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.1);
    transition: transform 0.3s, box-shadow 0.3s;
}

section:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 30px rgba(0,0,0,0.2);
}

section h2 {
    color: #ff69b4;
    margin-bottom: 20px;
    font-size: 2em;
}

section p {
    line-height: 1.6;
}

.prizes ul {
    list-style: none;
    padding: 0;
}

.prizes li {
    margin-bottom: 10px;
    font-weight: bold;
    animation: blink 1.5s infinite alternate;
}

@keyframes blink {
    0% { color: #ff69b4; }
    100% { color: #ff1493; }
}

/* Голосование — новогодняя коробочка */
.box-container {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    gap: 20px;
}

.box {
    width: 150px;
    height: 150px;
    background: linear-gradient(to bottom right, #ffb6c1, #ffe6f0);
    border-radius: 20px;
    text-align: center;
    padding: 15px;
    cursor: pointer;
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);
    position: relative;
    transition: transform 0.3s, box-shadow 0.3s;
}

.box:hover {
    transform: translateY(-10px) scale(1.05);
    box-shadow: 0 10px 30px rgba(0,0,0,0.3);
}

.box h3 {
    margin: 10px 0;
    color: #fff;
}

.box-bar {
    position: absolute;
    bottom: 0;
    left: 0;
    height: 15px;
    background: #ff69b4;
    border-radius: 0 0 20px 20px;
    width: 0%;
    transition: width 0.5s;
}

/* Соцсети */
.socials a {
    display: inline-block;
    margin-right: 15px;
    text-decoration: none;
    color: #fff;
    background-color: #ff69b4;
    padding: 10px 15px;
    border-radius: 10px;
    transition: background 0.3s;
}

.socials a:hover {
    background-color: #ff4d94;
}

footer {
    text-align: center;
    padding: 30px 20px;
    font-size: 0.9em;
    color: #555;
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
    0% { transform: translateY(0); }
    100% { transform: translateY(100vh); }
}
</style>
</head>
<body>

<header>
    <h1>Кастомная игра с pavvmew</h1>
    <p>Dead By Daylight | 25.12.2025 | Формат 4v1</p>
    <div class="timer" id="countdown"></div>
</header>

<section class="prizes">
    <h2>Призы</h2>
    <ul>
        <li>Милые брелочки</li>
        <li>Ручная открытка от pavvmew</li>
    </ul>
</section>

<section class="rules">
    <h2>Правила турнира</h2>
    <p>Завоюй зрительские симпатии! Собери новогодний лук, кидайся снежками, используй 5 генов, развесели зрителя и спаси как можно больше товарищей. После игры стороны меняются, и ты будешь киллером — прояви оригинальность!</p>
    <p>За себя голосовать нельзя. Секретный гость оценит игру и составит рейтинг. В случае равенства симпатий — спой или расскажи стих в Дискорде!</p>
    <p>Участвуй в "Лучший чаттерс": делай клипы, шутки и комментарии, чтобы заработать баллы.</p>
</section>

<section>
    <h2>Голосование зрителей</h2>
    <div class="box-container">
        <div class="box" onclick="vote('Игрок 1')">
            <h3>Игрок 1</h3>
            <div class="box-bar" id="Игрок1Bar"></div>
        </div>
        <div class="box" onclick="vote('Игрок 2')">
            <h3>Игрок 2</h3>
            <div class="box-bar" id="Игрок2Bar"></div>
        </div>
        <div class="box" onclick="vote('Игрок 3')">
            <h3>Игрок 3</h3>
            <div class="box-bar" id="Игрок3Bar"></div>
        </div>
    </div>
</section>

<section class="socials">
    <h2>Соцсети</h2>
    <a href="https://t.me/pavvmew" target="_blank">Telegram</a>
    <a href="https://www.tiktok.com/@pavvmi?_t=ZS-8zD1VOxHDUn&_r=1" target="_blank">TikTok</a>
    <a href="https://steamcommunity.com/id/pavvmi/" target="_blank">Steam</a>
</section>

<footer>
    © 2025 pavvmew | Все права защищены
</footer>

<script>
// Таймер
const countdown = document.getElementById('countdown');
const eventDate = new Date('2025-12-25T00:00:00');
function updateTimer() {
    const now = new Date();
    const diff = eventDate - now;
    if (diff <= 0) {
        countdown.textContent = "Турнир уже начался!";
        return;
    }
    const days = Math.floor(diff / (1000 * 60 * 60 * 24));
    const hours = Math.floor((diff / (1000 * 60 * 60)) % 24);
    const minutes = Math.floor((diff / 1000 / 60) % 60);
    const seconds = Math.floor((diff / 1000) % 60);
    countdown.textContent = `${days}д ${hours}ч ${minutes}м ${seconds}с`;
}
setInterval(updateTimer, 1000);
updateTimer();

// Голосование
const votes = { 'Игрок 1': 0, 'Игрок 2': 0, 'Игрок 3': 0 };
function vote(player) {
    votes[player]++;
    const total = votes['Игрок 1'] + votes['Игрок 2'] + votes['Игрок 3'];
    document.getElementById('Игрок1Bar').style.width = (votes['Игрок 1']/total*100) + '%';
    document.getElementById('Игрок2Bar').style.width = (votes['Игрок 2']/total*100) + '%';
    document.getElementById('Игрок3Bar').style.width = (votes['Игрок 3']/total*100) + '%';
}

// Снег
function createSnowflake() {
    const snowflake = document.createElement('div');
    snowflake.classList.add('snowflake');
    snowflake.textContent = '❄';
    snowflake.style.left = Math.random() * window.innerWidth + 'px';
    snowflake.style.fontSize = (Math.random()*20 + 10) + 'px';
    snowflake.style.animationDuration = (Math.random()*5 + 5) + 's';
    document.body.appendChild(snowflake);
    setTimeout(() => snowflake.remove(), 10000);
}
setInterval(createSnowflake, 200);
</script>

</body>
</html>
