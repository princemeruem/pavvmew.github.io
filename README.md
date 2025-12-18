
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Кастомная игра с pavvmew</title>
  <style>
    :root {
      --bg: linear-gradient(180deg, #ffffff, #ffe4e1);
      --card: rgba(255, 255, 255, 0.9);
      --text: #111;
      --muted: #555;
      --accent: #ff69b4;
    }
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background: var(--bg);
      color: var(--text);
    }
    header {
      padding: 80px 20px;
      text-align: center;
      background: radial-gradient(ellipse at top, #ffffff, transparent 70%);
    }
    header h1 {
      font-size: 3rem;
      margin: 0 0 10px;
    }
    header p {
      color: var(--muted);
      font-size: 1.2rem;
    }
    .container {
      max-width: 1000px;
      margin: 0 auto;
      padding: 40px 20px 80px;
      display: grid;
      gap: 32px;
    }
    .card {
      background: var(--card);
      border-radius: 20px;
      padding: 28px;
      box-shadow: 0 20px 40px rgba(0,0,0,0.2);
    }
    .card h2 {
      margin-top: 0;
      margin-bottom: 16px;
      font-size: 1.6rem;
    }
    ul {
      padding-left: 20px;
      margin: 0;
    }
    li {
      margin-bottom: 8px;
    }
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
      gap: 20px;
    }
    .prize {
      background: #fff0f5;
      border-radius: 16px;
      padding: 20px;
      border: 1px solid #ffc0cb;
    }
    .prize strong {
      color: var(--accent);
      font-size: 1.2rem;
    }
    footer {
      text-align: center;
      padding: 40px 20px;
      color: var(--muted);
      font-size: 0.9rem;
    }
    footer a {
      color: var(--accent);
      text-decoration: none;
      margin: 0 10px;
    }
    .btn {
      display: inline-block;
      margin-top: 24px;
      padding: 14px 28px;
      background: var(--accent);
      color: #fff;
      font-weight: 600;
      border-radius: 999px;
      text-decoration: none;
    }
  </style>
</head>
<body>

<header>
  <h1>Кастомная игра с pavvmew</h1>
  <p>Dead By Daylight • 25.12.2025 • Формат 4v1</p>
  <a href="#rules" class="btn">Смотреть правила</a>
</header>

<main class="container">

  <section class="card">
    <h2>Общая информация</h2>
    <p>
      Кастомная игра с pavvmew — уникальный онлайн-турнир по Dead By Daylight.
      Завоевывайте зрительские симпатии и получайте свои новогодние подарочки от pavvmew!
    </p>
  </section>

  <section class="card" id="rules">
    <h2>Правила</h2>
    <p>
      Твоя задача завоевать как можно больше зрительских симпатий!! Они смогут проголосовать за тебя, отдав свои баллы канала в твою новогоднюю коробочку ;)
      Собери интересный новогодний лук своему сурву, кидайся снежками, манси 5 генов, развесели зрителя своей игрой, при этом ты должен выиграть и спасти как можно больше товарищей.
      После игры за сурвов стороны меняются и ты обязательно будешь киллером, здесь твоя задача быть оригинальным (пробуй разные билды, манов, тактики) и сделать -3.
      По окончанию матчей мы подсчитаем количество заработанных симпатий (баллов канала) и отправим символический подарочек победителю почтой (вы должны проживать в РФ), если вы живете в другом месте, подарок будет цифровой :р.
      ЗА СЕБЯ голосовать нельзя (очевидно).
      Также наши катки будет комментировать секретный гость, который совсем ничего не понимает в игре и играл один раз в жизни, он также будет оценивать нашу игру и выставлять предварительный рейтинг самых крутых игроков (конечный выбор фаворита остается также за зрителем).
      Если количество симпатий у нескольких игроков совпадает, мы попросим каждого претендента рассказать нам новогодний стих/спеть новогоднюю песню в дискорд канале!
      Пока остальные веселят тебя в игре, ты можешь также поучаствовать в активности "лучший чаттерс" - делай забавные клипы, оригинально шути и комментируй происходящее, заливай свои баллы канала и активно проявляй себя. В конце стрима я и модератор определим победителя и отправим ему маленький подарок!
    </p>
  </section>

  <section class="card">
    <h2>Расписание</h2>
    <ul>
      <li>Дата проведения: 25 декабря 2025</li>
    </ul>
  </section>

  <section class="card">
    <h2>Награды</h2>
    <div class="grid">
      <div class="prize">
        <strong>Главный приз</strong>
        <p>Милые брелочки и ручная открытка от pavvmew</p>
      </div>
    </div>
  </section>

</main>

<footer>
  <p>Контакты организатора:</p>
  <a href="https://t.me/pavvmew" target="_blank">Telegram</a>
  <a href="https://www.tiktok.com/@pavvmi?_t=ZS-8zD1VOxHDUn&_r=1" target="_blank">TikTok</a>
  <a href="https://steamcommunity.com/id/pavvmi/" target="_blank">Steam</a>
</footer>

</body>
</html>
