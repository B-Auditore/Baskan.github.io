<html lang="tr">
<head>
  <meta charset="UTF-8">
  <title>Mervoş reis kusura bakma😞 al bu pasta sana 🎂</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #5A122A, #76B6E5);
      color: white;
      text-align: center;
      overflow-x: hidden;
    }
    h1 {
      margin-top: 20px;
      font-size: 2.5em;
    }
    p {
      font-size: 1.2em;
      margin-bottom: 20px;
    }
    .slideshow {
      max-width: 600px;
      margin: 20px auto;
      position: relative;
    }
    .slideshow img {
      width: 100%;
      border-radius: 20px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.5);
      display: none;
    }
    .slideshow img.active {
      display: block;
      animation: fade 2s;
    }
    @keyframes fade {
      from {opacity: 0.4;}
      to {opacity: 1;}
    }
    footer {
      margin-top: 20px;
      font-size: 0.9em;
      opacity: 0.8;
    }
  </style>
</head>
<body>
  <h1>🎂 Mervoş Doğum Günün Kutlu Olsun 🎂</h1>
  <p>Gurbetteyim gurbettee. İyi ki dogdun iyi ki varsın ❤️🧁🍫🍬🍭🍪🥮🎂 dur pastayı böleyim senin yerine 🍰 heh. Al sana kahve de ☕️. Bir de hediye vereyim 🎁. 🎁--> ⭐️(fenerden çaldım) gün bitmeden yetiştirmem lazım  </p>

  <div class="slideshow">
    <img src="mervos1.jpg" class="active" alt="Fotoğraf 1">
    <img src="mervos2.jpg" alt="Fotoğraf 2">
    <img src="mervos3.jpg" alt="Fotoğraf 3">
    <img src="mervos4.jpg" alt="Fotoğraf 4">
    <img src="mervos5.jpg" alt="Fotoğraf 5">
    <img src="mervos6.jpg" alt="Fotoğraf 6">
  </div>

  <!-- Oynatma Tuşu -->
<button onclick="playMusic()">Müziği Başlat</button>
<button onclick="pauseMusic()">Durdur</button>

<!-- Ses Dosyası -->
<audio id="arkamuzik" loop>
  <source src="muzik.mp3" type="audio/mpeg">
  Tarayıcınız audio elementini desteklemiyor.
</audio>

<script>
  const music = document.getElementById('arkamuzik');

  function playMusic() {
    music.play();
  }

  function pauseMusic() {
    music.pause();
  }
</script>

  <footer>Hazırlayan: Oruç ❤️</footer>

  <script>
    let index = 0;
    const images = document.querySelectorAll(".slideshow img");
    function showNext() {
      images[index].classList.remove("active");
      index = (index + 1) % images.length;
      images[index].classList.add("active");
    }
    setInterval(showNext, 4000);
  </script>
</body>
</html>
