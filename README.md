
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Кастомная игра с pavvmew | Dead By Daylight</title>
<link href="https://fonts.googleapis.com/css2?family=Indie+Flower&display=swap" rel="stylesheet">
<style>
body {
    margin: 0;
    font-family: 'Indie Flower', cursive;
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

section h2, .features h3, .rewards h3, .gifts h3 {
    color: #ff1493;
    margin-bottom: 15px;
    text-align: center;
}

section p {
    line-height: 1.6;
    font-size: 1.2em;
    margin-bottom: 15px;
}

.underline {
    text-decoration: underline;
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

/* Особенности, подарки, награды */
.features, .gifts, .rewards {
    background: rgba(255, 255, 255, 0.95);
    padding: 20px 25px;
    border-radius: 20px;
    margin: 30px auto;
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);
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
    <p>Твоя задача сегодня - завоевать как можно больше зрительских симпатий! Они смогут проголосовать за тебя, отдав свои баллы канала в твой новогодний подарок ;)</p>
    <p>Собирай свой оригинальный новогодний лук в лобби, кидайся снежками, авантюрно отбегай злого деда Мороза 5 генераторов, тибагай, кивай, тверкай в паллетах, но не забывай о том, что тебе также нужно спасти как можно больше товарищей.</p>
    <p>После игры за сурвов стороны меняются, и ты обязательно будешь злым дедом Морозом. Здесь твоя задача - проявить креативность (пробуй необычные/странные/забавные билды, редких манов, интересные или не очень тактики) и конечно наказать минимум трех непослушных оленей.</p>
    <p>Я буду играть вместе с вами как за оленей, так и за деда Мороза, поэтому чтобы твои шалости были замечены и оценены во время игры со мной, чаще попадайся нам со зрителями на глаза!</p>
    <p>По окончанию матчей мы подсчитаем количество заслуженных симпатий (баллов канала) и определим победителя!</p>
    <p>Но, это еще не все. Пока остальные веселят тебя в игре, ты можешь также поучаствовать в активности <span class="underline">"лучший чаттерс"</span> - здесь твоя задача проста: делай клипы забавных моментов, оригинально шути и комментируй происходящее, заливай свои баллы канала и активно проявляй себя. В конце стрима я и модератор определим победителя (если ты также играешь с нами в кастомке, у тебя есть возможность залутать несколько наград).</p>
</section>

<section class="features">
    <h3>Особенности</h3>
    <p>Наши игры будет комментировать <span class="underline">новогодний кролик</span>, только он совсем не смыслит ничего в наших играх, поэтому будет выступать символом веселья и радости. Ему также поручено оценивать матчи и помогать мне выставлять предварительный рейтинг самых крутых игроков, однако конечный выбор победителя остается также за зрителем!</p>
    <p>За <span class="underline">СЕБЯ</span> голосовать нельзя :Р</p>
    <p>В случае, если у игроков будет равное количество симпатий, мы попросим кандидатов на подарок рассказать нам <span class="underline">новогодний стих</span> или <span class="underline">спеть новогоднюю песню</span>.</p>
</section>

<section class="gifts">
    <h3>Подарки от pavvmew</h3>
    <p>Победитель награждается символическим призом: милый брелок с котиком, лапка сквиш и ручная открытка с новогодним поздравлением от меня &lt;3 (отправление почтой РФ, если вы здесь не живете, подарок будет в виде мини-арта от меня на любую выбранную вами тему, либо на мой выбор) &lt;3</p>
</section>

<section class="rewards">
    <h3>Награды за баллы канала</h3>
    <p>100 лапок - твоя симпатия игроку, который вызвал у тебя приятные эмоции</p>
    <p>Минимум 100, максимум 3000 лапок (баллов канала) на одного игрока</p>
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
