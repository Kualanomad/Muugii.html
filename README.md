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
      background: url('https://images.unsplash.com/photo-1509228627152-72ae9ae6848c') no-repeat center center fixed;
      background-size: cover;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      text-align: center;
      overflow: hidden;
    }
    .card {
      background: rgba(255, 255, 255, 0.9);
      padding: 2rem;
      border-radius: 1.5rem;
      box-shadow: 0 10px 30px rgba(0,0,0,0.3);
      max-width: 400px;
      animation: fadeIn 2s ease-in;
    }
    h1 {
      color: #ff1493;
      animation: bounce 1.5s infinite;
    }
    .message {
      font-size: 1.2rem;
      margin-top: 1rem;
      color: #333;
    }
    .btn {
      display: inline-block;
      margin-top: 2rem;
      padding: 0.75rem 1.5rem;
      background: #ff1493;
      color: white;
      border: none;
      border-radius: 1rem;
      cursor: pointer;
      font-size: 1rem;
      transition: background 0.3s;
    }
    .btn:hover {
      background: #ff69b4;
    }
    .hidden {
      display: none;
    }
    @keyframes bounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }
    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }
  </style>
</head>
<body>
  <audio autoplay loop>
    <source src="https://www.bensound.com/bensound-music/bensound-happyrock.mp3" type="audio/mpeg">
    Таны хөтөч дуу тоглуулах боломжгүй байна.
  </audio>

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
