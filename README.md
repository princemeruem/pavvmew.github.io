# pavvmew.github.io
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Турнир</title>
  <style>
    :root {
      --bg: #0f172a;
      --card: #111827;
      --text: #e5e7eb;
      --muted: #9ca3af;
      --accent: #22c55e;
    }
    * { box-sizing: border-box; }
    body {
      margin: 0;
      font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI", sans-serif;
      background: linear-gradient(180deg, #020617, #020617 40%, #020617);
      color: var(--text);
    }
    header {
      padding: 80px 20px;
      text-align: center;
      background: radial-gradient(ellipse at top, #1e293b, transparent 70%);
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
      background: rgba(17,24,39,0.9);
      border: 1px solid #1f2937;
      border-radius: 20px;
      padding: 28px;
      box-shadow: 0 20px 40px rgba(0,0,0,0.4);
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
      background: #020617;
      border-radius: 16px;
      padding: 20px;
      border: 1px solid #1f2937;
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
    .btn {
      display: inline-block;
      margin-top: 24px;
      padding: 14px 28px;
      background: var(--accent);
      color: #020617;
      font-weight: 600;
      border-radius: 999px;
      text-decoration: none;
    }
  </style>
</head>
<body>

<header>
  <h1>Название турнира</h1>
  <p>Краткое описание турнира: формат, игра, даты</p>
  <a href="#rules" class="btn">Смотреть правила</a>
</header>

<main class="container">

  <section class="card">
    <h2>Общая информация</h2>
    <p>
      Здесь ты описываешь, что это за турнир, для кого он,
      сколько участников, онлайн или офлайн, даты и формат.
    </p>
  </section>

  <section class="card" id="rules">
    <h2>Правила</h2>
    <ul>
      <li>Условие участия</li>
      <li>Формат матчей</li>
      <li>Запрещённые действия</li>
      <li>Система побед и выбывания</li>
      <li>Решение спорных ситуаций</li>
    </ul>
  </section>

  <section class="card">
    <h2>Расписание</h2>
    <ul>
      <li>Регистрация: 1–10 мая</li>
      <li>Групповой этап: 12–15 мая</li>
      <li>Плей-офф: 17–18 мая</li>
      <li>Финал: 20 мая</li>
    </ul>
  </section>

  <section class="card">
    <h2>Награды</h2>
    <div class="grid">
      <div class="prize">
        <strong>1 место</strong>
        <p>Главный приз</p>
      </div>
      <div class="prize">
        <strong>2 место</strong>
        <p>Приз за второе место</p>
      </div>
      <div class="prize">
        <strong>3 место</strong>
        <p>Приз за третье место</p>
      </div>
    </div>
  </section>

</main>

<footer>
  <p>Контакты организатора · Discord / Telegram / Email</p>
</footer>

</body>
</html>
