<!DOCTYPE html>
<html lang="uk">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Бандерогусь</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(to bottom, #e6f0ff, #ffffff);
    }

    header {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
      padding: 40px 20px;
      background: white;
    }

    .content {
      max-width: 500px;
      margin: 20px;
      text-align: center;
    }

    .logo {
      font-weight: bold;
      font-size: 18px;
      margin-bottom: 10px;
    }

    h1 {
      font-size: 36px;
      margin: 10px 0;
    }

    .subtext {
      font-size: 16px;
      margin-bottom: 20px;
    }

    .button {
      background-color: orange;
      color: white;
      padding: 12px 24px;
      border: none;
      border-radius: 8px;
      font-size: 16px;
      cursor: pointer;
    }

    .goose-img img {
      max-width: 220px;
      margin: 20px auto;
    }

    .facts {
      padding: 40px 20px;
      text-align: center;
    }

    .facts h2 {
      font-size: 28px;
      margin-bottom: 20px;
    }

    .fact-items {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      margin-top: 30px;
    }

    .fact {
      width: 260px;
      text-align: center;
    }

    .fact img {
      max-width: 80px;
      margin-bottom: 10px;
    }

    .fact-title {
      font-weight: bold;
      margin-bottom: 8px;
    }

    .form-block {
      background: linear-gradient(to top, #cde9ff, #ffffff);
      padding: 40px 20px;
      text-align: center;
    }

    .form-container {
      max-width: 400px;
      margin: 0 auto;
      background: white;
      padding: 30px;
      border-radius: 16px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    }

    .form-container h3 {
      margin-bottom: 10px;
    }

    input[type="text"],
    input[type="email"] {
      width: 100%;
      padding: 10px;
      margin: 8px 0;
      border: 1px solid #ccc;
      border-radius: 8px;
    }

    .form-container button {
      background-color: orange;
      color: white;
      padding: 12px 24px;
      border: none;
      border-radius: 8px;
      font-size: 16px;
      cursor: pointer;
      margin-top: 10px;
    }

    @media (max-width: 600px) {
      h1 {
        font-size: 28px;
      }

      .subtext {
        font-size: 14px;
      }

      .facts h2 {
        font-size: 24px;
      }

      .fact {
        width: 90%;
      }

      .goose-img img {
        max-width: 180px;
      }
    }
  </style>
</head>
<body>

<header>
  <div class="content">
    <div class="logo">GO IT</div>
    <h1>Бандерогусь</h1>
    <p class="subtext">Добрий вечір, ми з України! Спеціальний бойовий гусак із Бандерівської України. Захищає державу, кряче «Слава Україні!» і заряджає бойовим духом!</p>
    <button class="button" onclick="playGoose()">Запустити гуся</button>
  </div>
  <div class="goose-img">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/63/Banderogoose.png/600px-Banderogoose.png" alt="Гусак">
  </div>
</header>

<section class="facts">
  <h2>Цікаві факти про бандерогусей</h2>
  <div class="fact-items">
    <div class="fact">
      <img src="https://img.icons8.com/ios/100/navigation.png" alt="GPS">
      <div class="fact-title">Система навігації</div>
      <p>Знаходить зрадників навіть уночі без ліхтарика.</p>
    </div>
    <div class="fact">
      <img src="https://img.icons8.com/ios/100/thermal-vision.png" alt="Тепловізор">
      <div class="fact-title">Очі-тепловізори</div>
      <p>Розпізнає ворога за температурою духу.</p>
    </div>
    <div class="fact">
      <img src="https://img.icons8.com/ios/100/jet.png" alt="Байракрилата">
      <div class="fact-title">Байракрилата</div>
      <p>Атакує на всіх фронтах, навіть у TikTok.</p>
    </div>
  </div>
</section>

<section class="form-block">
  <div class="form-container">
    <h3>Поділися, будь ласка, поштою</h3>
    <p>та запишись до фан-клубу бандерогуся!</p>
    <form>
      <input type="text" placeholder="Ім'я">
      <input type="email" placeholder="Email">
      <button type="submit">Записатись!</button>
    </form>
  </div>
</section>

<audio id="gooseSound" src="643-slava-ukrayini-gurt-kuli.mp3" preload="auto"></audio>

<script>
  function playGoose() {
    const sound = document.getElementById('gooseSound');
    sound.currentTime = 0;
    sound.play();
  }
</script>

</body>
</html>
