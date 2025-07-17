# Muugii.html
My Dear Friend
<!DOCTYPE html>
<html lang="mn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Төрсөн өдрийн мэнд!</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Arial', sans-serif;
      background: linear-gradient(135deg, #ffd1dc, #ffe4e1);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      text-align: center;
    }
    .card {
      background: white;
      padding: 2rem;
      border-radius: 1.5rem;
      box-shadow: 0 10px 30px rgba(0,0,0,0.2);
      max-width: 400px;
    }
    h1 {
      color: #ff69b4;
    }
    .message {
      font-size: 1.2rem;
      margin-top: 1rem;
      color: #555;
    }
    .btn {
      display: inline-block;
      margin-top: 2rem;
      padding: 0.75rem 1.5rem;
      background: #ff69b4;
      color: white;
      border: none;
      border-radius: 1rem;
      cursor: pointer;
      font-size: 1rem;
    }
    .hidden {
      display: none;
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>Төрсөн өдрийн мэнд, найзаа! 🎉</h1>
    <p class="message" id="msg">Өнөөдөр чиний онцгой өдөр. Бэлгээ нээхэд бэлэн үү?</p>
    <button class="btn" onclick="revealGift()">Бэлэг нээх 🎁</button>
    <p class="message hidden" id="giftMsg">Сюрприз! Чамд аз жаргал, инээд баясал бэлэглэе! 🥳</p>
  </div>

  <script>
    function revealGift() {
      document.getElementById('msg').classList.add('hidden');
      document.querySelector('.btn').classList.add('hidden');
      document.getElementById('giftMsg').classList.remove('hidden');
    }
  </script>
</body>
</html>
